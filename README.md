<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ชมรมหุ่นยนต์โรงเรียน (Robot Club)</title>
    
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Sarabun:wght@300;400;600;700&display=swap" rel="stylesheet">

    <style>
        /* --- ตั้งค่าพื้นฐาน (Reset & Global Styles) --- */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Sarabun', sans-serif;
        }

        body {
            background-color: #F9FBF9;
            color: #333;
            line-height: 1.6;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 40px 20px;
        }

        h2 {
            text-align: center;
            color: #2E7D32;
            margin-bottom: 30px;
            font-size: 2rem;
            position: relative;
        }

        h2::after {
            content: '';
            display: block;
            width: 60px;
            height: 4px;
            background-color: #4CAF50;
            margin: 10px auto 0;
            border-radius: 2px;
        }

        section {
            margin-bottom: 40px;
        }

        /* --- Hero Banner --- */
        .hero {
            background: linear-gradient(135deg, #4CAF50 0%, #1B5E20 100%);
            color: white;
            text-align: center;
            padding: 100px 20px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        .hero-icon {
            font-size: 5rem;
            margin-bottom: 15px;
            animation: float 3s ease-in-out infinite;
        }

        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }

        .hero h1 {
            font-size: 3rem;
            font-weight: 700;
            margin-bottom: 10px;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .hero p {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 60px;
            max-width: 600px;
            margin: 0 auto;
        }

        /* --- Activities Section (3-Column Cards) --- */
        .activity-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
            margin-top: 20px;
        }

        .card {
            background: #FFFFFF;
            border-radius: 12px;
            padding: 30px 20px;
            text-align: center;
            border: 1px solid #E8F5E9;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 15px rgba(76, 175, 80, 0.2);
        }

        .card-icon {
            font-size: 3.5rem;
            margin-bottom: 15px;
        }

        .card h3 {
            color: #1B5E20;
            margin-bottom: 12px;
            font-size: 1.3rem;
        }

        .card p {
            color: #666;
            font-size: 0.95rem;
        }

        /* --- Schedule Table Section --- */
        .table-responsive {
            overflow-x: auto;
            background: #FFFFFF;
            border-radius: 12px;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            border: 1px solid #E8F5E9;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            text-align: left;
        }

        th, td {
            padding: 15px 20px;
        }

        th {
            background-color: #4CAF50;
            color: white;
            font-weight: 600;
        }

        tr:nth-child(even) {
            background-color: #E8F5E9; /* Zebra Striping */
        }

        tr:hover {
