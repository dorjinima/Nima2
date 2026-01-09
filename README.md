<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Druk Journey | Bhutan Travel Specialists</title>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@400;500;600;700&display=swap" rel="stylesheet">
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Favicon -->
    <link rel="icon" type="image/x-icon" href="#">
    <style>
        /* CSS Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-color: #ff6b35; /* Bhutan orange */
            --primary-dark: #e55a2b;
            --secondary-color: #1a472a; /* Bhutan green */
            --accent-color: #f4c542; /* Bhutan gold */
            --light-color: #f8f9fa;
            --dark-color: #2c3e50;
            --gray-color: #6c757d;
            --shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            --transition: all 0.3s ease;
            --border-radius: 8px;
            --dragon-red: #d32f2f;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: var(--dark-color);
            background-color: #fff;
            overflow-x: hidden;
        }

        h1, h2, h3, h4 {
            font-family: 'Montserrat', sans-serif;
            font-weight: 600;
            line-height: 1.3;
            margin-bottom: 1rem;
        }

        h1 {
            font-size: 2.8rem;
        }

        h2 {
            font-size: 2.2rem;
            color: var(--secondary-color);
            position: relative;
            padding-bottom: 15px;
            margin-bottom: 2rem;
        }

        h2:after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: var(--primary-color);
            border-radius: 2px;
        }

        h3 {
            font-size: 1.5rem;
            color: var(--secondary-color);
        }

        p {
            margin-bottom: 1rem;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        ul {
            list-style: none;
        }

        img {
            max-width: 100%;
            height: auto;
            display: block;
        }

        section {
            padding: 80px 0;
        }

        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        .btn {
            display: inline-block;
            padding: 12px 30px;
            background-color: var(--primary-color);
            color: white;
            border: none;
            border-radius: var(--border-radius);
            cursor: pointer;
            font-weight: 600;
            font-size: 1rem;
            transition: var(--transition);
            text-align: center;
        }

        .btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-3px);
            box-shadow: var(--shadow);
        }

        .btn-secondary {
            background-color: var(--accent-color);
            color: var(--dark-color);
        }

        .btn-secondary:hover {
            background-color: #e0b73a;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
        }

        .section-title p {
            max-width: 700px;
            margin: 0 auto;
            color: var(--gray-color);
        }

        /* Header & Navbar */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            z-index: 1000;
            background-color: rgba(255, 255, 255, 0.95);
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
            transition: var(--transition);
        }

        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--secondary-color);
            display: flex;
            align-items: center;
        }

        .logo i {
            margin-right: 8px;
            font-size: 1.6rem;
            color: var(--dragon-red);
        }

        .nav-links {
            display: flex;
            gap: 30px;
        }

        .nav-links a {
            font-weight: 500;
            color: var(--dark-color);
            transition: var(--transition);
            position: relative;
        }

        .nav-links a:hover, .nav-links a.active {
            color: var(--primary-color);
        }

        .nav-links a.active:after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 100%;
            height: 2px;
            background-color: var(--primary-color);
        }

        .hamburger {
            display: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--dark-color);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('https://images.unsplash.com/photo-1580737661251-9d1c8543b0c4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80');
            background-size: cover;
            background-position: center;
            color: white;
            min-height: 100vh;
            display: flex;
            align-items: center;
            text-align: center;
            position: relative;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
            position: relative;
            z-index: 2;
        }

        .hero h1 {
            font-size: 3.5rem;
            margin-bottom: 1.5rem;
            color: white;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2.5rem;
            opacity: 0.9;
        }

        .hero .btn {
            margin-top: 1rem;
        }

        /* Bhutan Flag Element */
        .bhutan-flag {
            display: flex;
            justify-content: center;
            margin: 30px 0;
        }

        .flag-part {
            width: 50px;
            height: 30px;
            margin: 0 5px;
        }

        .flag-orange {
            background-color: var(--primary-color);
        }

        .flag-yellow {
            background-color: var(--accent-color);
        }

        .flag-dragon {
            font-size: 24px;
            color: white;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: var(--dragon-red);
            border-radius: 50%;
            width: 40px;
            height: 40px;
            margin: 0 10px;
        }

        /* Visa Info Box */
        .visa-info {
            background-color: rgba(255, 255, 255, 0.9);
            color: var(--secondary-color);
            padding: 20px;
            border-radius: var(--border-radius);
            margin-top: 30px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        .visa-info h4 {
            color: var(--primary-color);
            margin-bottom: 10px;
        }

        /* Enhanced Booking Form */
        .booking-form-container {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 40px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
            margin-top: 40px;
            max-width: 1000px;
            margin-left: auto;
            margin-right: auto;
        }

        .form-header {
            text-align: center;
            margin-bottom: 30px;
        }

        .form-header h3 {
            color: var(--primary-color);
            font-size: 1.8rem;
        }

        .form-header p {
            color: var(--gray-color);
        }

        .form-progress {
            display: flex;
            justify-content: space-between;
            margin-bottom: 40px;
            position: relative;
        }

        .form-progress:before {
            content: '';
            position: absolute;
            top: 15px;
            left: 0;
            width: 100%;
            height: 3px;
            background-color: #e0e0e0;
            z-index: 1;
        }

        .progress-step {
            display: flex;
            flex-direction: column;
            align-items: center;
            position: relative;
            z-index: 2;
        }

        .step-number {
            width: 35px;
            height: 35px;
            background-color: #e0e0e0;
            color: var(--dark-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-weight: 600;
            margin-bottom: 10px;
            transition: var(--transition);
        }

        .progress-step.active .step-number {
            background-color: var(--primary-color);
            color: white;
            transform: scale(1.1);
        }

        .progress-step.completed .step-number {
            background-color: var(--secondary-color);
            color: white;
        }

        .step-label {
            font-size: 0.9rem;
            font-weight: 500;
            color: var(--gray-color);
        }

        .progress-step.active .step-label {
            color: var(--primary-color);
            font-weight: 600;
        }

        .form-step {
            display: none;
            animation: fadeIn 0.5s ease;
        }

        .form-step.active {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .form-row {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-bottom: 25px;
        }

        .form-group {
            display: flex;
            flex-direction: column;
        }

        .form-group label {
            margin-bottom: 8px;
            font-weight: 500;
            color: var(--secondary-color);
            display: flex;
            align-items: center;
        }

        .form-group label i {
            margin-right: 8px;
            color: var(--primary-color);
        }

        .form-control {
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: var(--border-radius);
            font-family: 'Poppins', sans-serif;
            font-size: 1rem;
            transition: var(--transition);
        }

        .form-control:focus {
            outline: none;
            border-color: var(--primary-color);
            box-shadow: 0 0 0 2px rgba(255, 107, 53, 0.2);
        }

        .form-actions {
            display: flex;
            justify-content: space-between;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #eee;
        }

        .form-note {
            background-color: #f9f9f9;
            padding: 15px;
            border-radius: var(--border-radius);
            margin-top: 20px;
            font-size: 0.9rem;
            color: var(--gray-color);
            border-left: 3px solid var(--accent-color);
        }

        .form-note i {
            color: var(--accent-color);
            margin-right: 8px;
        }

        .error-message {
            color: var(--dragon-red);
            font-size: 0.85rem;
            margin-top: 5px;
            display: none;
        }

        /* Tours Section */
        .filters {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }

        .filter-btn {
            padding: 8px 20px;
            background-color: #f1f1f1;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            font-weight: 500;
            transition: var(--transition);
        }

        .filter-btn.active, .filter-btn:hover {
            background-color: var(--primary-color);
            color: white;
        }

        .tour-cards {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }

        .tour-card {
            background-color: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border-top: 4px solid var(--primary-color);
        }

        .tour-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.15);
        }

        .tour-img {
            height: 200px;
            overflow: hidden;
        }

        .tour-img img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: var(--transition);
        }

        .tour-card:hover .tour-img img {
            transform: scale(1.05);
        }

        .tour-content {
            padding: 20px;
        }

        .tour-header {
            display: flex;
            justify-content: space-between;
            align-items: flex-start;
            margin-bottom: 10px;
        }

        .tour-price {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-color);
        }

        .tour-duration {
            display: flex;
            align-items: center;
            color: var(--gray-color);
            font-size: 0.9rem;
        }

        .tour-duration i {
            margin-right: 5px;
        }

        .tour-rating {
            display: flex;
            align-items: center;
            margin-top: 10px;
        }

        .tour-rating i {
            color: var(--accent-color);
            margin-right: 2px;
        }

        .tour-rating span {
            margin-left: 8px;
            color: var(--gray-color);
        }

        /* Hotels Section */
        .hotel-cards {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }

        .hotel-card {
            background-color: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            border-top: 4px solid var(--accent-color);
        }

        .hotel-content {
            padding: 20px;
        }

        .hotel-price {
            font-size: 1.3rem;
            font-weight: 700;
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        .hotel-price span {
            font-size: 0.9rem;
            font-weight: normal;
            color: var(--gray-color);
        }

        .price-calculator {
            background-color: #f9f9f9;
            border-radius: var(--border-radius);
            padding: 30px;
            box-shadow: var(--shadow);
        }

        .calculation-result {
            background-color: white;
            padding: 20px;
            border-radius: var(--border-radius);
            margin-top: 20px;
            border: 1px solid #eee;
            display: none;
        }

        .total-price {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary-color);
            margin-top: 10px;
        }

        /* Trekking Packages */
        .trekking-packages {
            background-color: #f9f9f9;
        }

        .package-cards {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }

        .package-card {
            background-color: white;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
            border-top: 4px solid var(--secondary-color);
        }

        .difficulty {
            display: inline-block;
            padding: 4px 12px;
            background-color: var(--accent-color);
            color: var(--dark-color);
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 600;
            margin-top: 10px;
        }

        /* Enhanced Vehicle Section */
        .vehicle-section {
            background-color: #f9f9f9;
        }

        .vehicle-filters {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-bottom: 40px;
            flex-wrap: wrap;
        }

        .vehicle-filter-btn {
            padding: 8px 20px;
            background-color: #f1f1f1;
            border: none;
            border-radius: 30px;
            cursor: pointer;
            font-weight: 500;
            transition: var(--transition);
        }

        .vehicle-filter-btn.active, .vehicle-filter-btn:hover {
            background-color: var(--primary-color);
            color: white;
        }

        .vehicle-cards {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 30px;
            margin-bottom: 40px;
        }

        .vehicle-card {
            background-color: white;
            border-radius: var(--border-radius);
            padding: 25px;
            text-align: center;
            box-shadow: var(--shadow);
            transition: var(--transition);
            border-top: 4px solid var(--primary-color);
            display: flex;
            flex-direction: column;
            height: 100%;
        }

        .vehicle-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
        }

        .vehicle-icon {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 15px;
        }

        .vehicle-price {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-color);
            margin: 15px 0;
        }

        .vehicle-features {
            list-style: none;
            text-align: left;
            margin: 15px 0;
            flex-grow: 1;
        }

        .vehicle-features li {
            margin-bottom: 8px;
            display: flex;
            align-items: center;
        }

        .vehicle-features i {
            color: var(--primary-color);
            margin-right: 10px;
            font-size: 0.9rem;
        }

        .vehicle-actions {
            display: flex;
            gap: 10px;
            margin-top: 20px;
        }

        .vehicle-actions .btn {
            flex: 1;
        }

        /* Cultural Experiences */
        .culture-cards {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 30px;
        }

        .culture-card {
            text-align: center;
            padding: 30px 20px;
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            transition: var(--transition);
        }

        .culture-card:hover {
            transform: translateY(-5px);
        }

        .culture-icon {
            font-size: 2.5rem;
            color: var(--primary-color);
            margin-bottom: 20px;
        }

        /* Testimonials */
        .testimonials-container {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
            overflow: hidden;
        }

        .testimonial-slider {
            display: flex;
            transition: transform 0.5s ease;
        }

        .testimonial {
            min-width: 100%;
            padding: 40px;
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
            text-align: center;
        }

        .client-img {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            object-fit: cover;
            margin: 0 auto 20px;
            border: 3px solid var(--primary-color);
        }

        .client-rating {
            color: var(--accent-color);
            margin: 15px 0;
        }

        .slider-controls {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 30px;
        }

        .slider-btn {
            background-color: var(--primary-color);
            color: white;
            width: 40px;
            height: 40px;
            border-radius: 50%;
            border: none;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }

        .slider-btn:hover {
            background-color: var(--primary-dark);
        }

        /* Contact Section */
        .contact-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 40px;
        }

        .contact-info {
            display: flex;
            flex-direction: column;
            gap: 20px;
        }

        .contact-item {
            display: flex;
            align-items: flex-start;
            gap: 15px;
        }

        .contact-icon {
            background-color: var(--primary-color);
            color: white;
            width: 50px;
            height: 50px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            flex-shrink: 0;
        }

        .contact-form {
            background-color: white;
            padding: 30px;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
        }

        .map-container {
            height: 300px;
            margin-top: 30px;
            border-radius: var(--border-radius);
            overflow: hidden;
            box-shadow: var(--shadow);
        }

        .map-container iframe {
            width: 100%;
            height: 100%;
            border: none;
        }

        /* Footer */
        footer {
            background-color: var(--secondary-color);
            color: white;
            padding: 60px 0 30px;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }

        .footer-logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: white;
            margin-bottom: 20px;
            display: flex;
            align-items: center;
        }

        .footer-logo i {
            margin-right: 8px;
            color: var(--dragon-red);
        }

        .footer-about p {
            margin-bottom: 20px;
            opacity: 0.8;
        }

        .social-icons {
            display: flex;
            gap: 15px;
        }

        .social-icon {
            display: flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            transition: var(--transition);
        }

        .social-icon:hover {
            background-color: var(--primary-color);
            transform: translateY(-3px);
        }

        .footer-links h3, .footer-newsletter h3 {
            font-size: 1.3rem;
            margin-bottom: 25px;
            color: white;
        }

        .footer-links ul {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .footer-links a {
            opacity: 0.8;
            transition: var(--transition);
        }

        .footer-links a:hover {
            opacity: 1;
            color: var(--accent-color);
            padding-left: 5px;
        }

        .newsletter-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0.7;
            font-size: 0.9rem;
        }

        /* Modal */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            z-index: 2000;
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            background-color: white;
            border-radius: var(--border-radius);
            width: 90%;
            max-width: 600px;
            max-height: 90vh;
            overflow-y: auto;
            padding: 30px;
            position: relative;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }

        .modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            background: none;
            border: none;
            font-size: 1.5rem;
            cursor: pointer;
            color: var(--gray-color);
            transition: var(--transition);
        }

        .modal-close:hover {
            color: var(--dark-color);
        }

        .modal h3 {
            margin-bottom: 20px;
            color: var(--primary-color);
        }

        /* Enhanced Chat Bot */
        .chatbot-container {
            position: fixed;
            bottom: 20px;
            right: 20px;
            z-index: 1001;
        }

        .chatbot-toggle {
            width: 60px;
            height: 60px;
            background-color: var(--primary-color);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            font-size: 1.5rem;
            cursor: pointer;
            box-shadow: 0 4px 15px rgba(255, 107, 53, 0.4);
            transition: var(--transition);
        }

        .chatbot-toggle:hover {
            background-color: var(--primary-dark);
            transform: scale(1.05);
        }

        .chatbot-window {
            position: absolute;
            bottom: 70px;
            right: 0;
            width: 400px;
            height: 600px;
            background-color: white;
            border-radius: var(--border-radius);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            display: none;
            flex-direction: column;
            overflow: hidden;
        }

        .chatbot-header {
            background-color: var(--secondary-color);
            color: white;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .chatbot-header h3 {
            color: white;
            margin: 0;
            font-size: 1.2rem;
            display: flex;
            align-items: center;
        }

        .chatbot-header h3 i {
            margin-right: 10px;
        }

        .chatbot-close {
            background: none;
            border: none;
            color: white;
            font-size: 1.2rem;
            cursor: pointer;
        }

        .chatbot-messages {
            flex: 1;
            padding: 20px;
            overflow-y: auto;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .chatbot-input {
            padding: 15px;
            border-top: 1px solid #eee;
            display: flex;
            gap: 10px;
            background-color: #f9f9f9;
        }

        .chatbot-input input {
            flex: 1;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 20px;
            font-family: 'Poppins', sans-serif;
            font-size: 0.9rem;
        }

        .chatbot-input button {
            background-color: var(--primary-color);
            color: white;
            border: none;
            border-radius: 50%;
            width: 40px;
            height: 40px;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }

        .chatbot-input button:hover {
            background-color: var(--primary-dark);
        }

        .message {
            max-width: 80%;
            padding: 12px 15px;
            border-radius: 18px;
            font-size: 0.9rem;
            line-height: 1.4;
        }

        .bot-message {
            background-color: #f1f1f1;
            align-self: flex-start;
            border-bottom-left-radius: 5px;
        }

        .user-message {
            background-color: var(--primary-color);
            color: white;
            align-self: flex-end;
            border-bottom-right-radius: 5px;
        }

        .quick-replies {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 10px;
        }

        .quick-reply {
            background-color: white;
            border: 1px solid var(--primary-color);
            color: var(--primary-color);
            padding: 6px 12px;
            border-radius: 20px;
            font-size: 0.8rem;
            cursor: pointer;
            transition: var(--transition);
        }

        .quick-reply:hover {
            background-color: var(--primary-color);
            color: white;
        }

        /* Bhutan Specials */
        .bhutan-special {
            background-color: #f9f9f9;
        }

        .special-item {
            display: flex;
            align-items: center;
            gap: 20px;
            margin-bottom: 30px;
            background-color: white;
            padding: 20px;
            border-radius: var(--border-radius);
            box-shadow: var(--shadow);
        }

        .special-icon {
            font-size: 2rem;
            color: var(--primary-color);
            min-width: 60px;
            text-align: center;
        }

        /* Booking Summary */
        .booking-summary {
            background-color: #f9f9f9;
            padding: 20px;
            border-radius: var(--border-radius);
            margin-top: 20px;
        }

        .summary-item {
            display: flex;
            justify-content: space-between;
            margin-bottom: 10px;
            padding-bottom: 10px;
            border-bottom: 1px solid #eee;
        }

        .summary-total {
            font-weight: 700;
            font-size: 1.2rem;
            color: var(--primary-color);
            margin-top: 10px;
            padding-top: 10px;
            border-top: 2px solid #ddd;
        }

        /* Responsive Styles */
        @media (max-width: 992px) {
            h1 {
                font-size: 2.5rem;
            }
            
            h2 {
                font-size: 2rem;
            }
            
            section {
                padding: 60px 0;
            }
            
            .chatbot-window {
                width: 350px;
                height: 500px;
            }
        }

        @media (max-width: 768px) {
            .hamburger {
                display: block;
            }
            
            .nav-links {
                position: fixed;
                top: 80px;
                left: 0;
                width: 100%;
                background-color: white;
                flex-direction: column;
                align-items: center;
                padding: 20px 0;
                box-shadow: 0 10px 15px rgba(0, 0, 0, 0.1);
                transform: translateY(-100%);
                opacity: 0;
                transition: var(--transition);
                z-index: 1000;
            }
            
            .nav-links.active {
                transform: translateY(0);
                opacity: 1;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .booking-form-container {
                padding: 25px;
            }
            
            .form-row {
                grid-template-columns: 1fr;
            }
            
            .tour-cards, .hotel-cards, .package-cards, .vehicle-cards, .culture-cards {
                grid-template-columns: 1fr;
            }
            
            .vehicle-actions {
                flex-direction: column;
            }
            
            .chatbot-window {
                width: 300px;
                height: 450px;
            }
        }

        @media (max-width: 576px) {
            h1 {
                font-size: 2rem;
            }
            
            h2 {
                font-size: 1.8rem;
            }
            
            .hero {
                min-height: 80vh;
            }
            
            .booking-form-container {
                padding: 20px;
            }
            
            .testimonial {
                padding: 30px 20px;
            }
            
            .form-progress {
                margin-bottom: 30px;
            }
            
            .step-label {
                font-size: 0.8rem;
            }
            
            .chatbot-window {
                width: calc(100vw - 40px);
                right: -10px;
            }
        }
    </style>
</head>
<body>
    <!-- Header & Navbar -->
    <header>
        <div class="container">
            <nav class="navbar">
                <a href="#" class="logo"><i class="fas fa-dragon"></i> Druk Journey</a>
                <div class="hamburger" id="hamburger">
                    <i class="fas fa-bars"></i>
                </div>
                <ul class="nav-links" id="navLinks">
                    <li><a href="#home" class="active">Home</a></li>
                    <li><a href="#tours">Bhutan Tours</a></li>
                    <li><a href="#trekking">Trekking</a></li>
                    <li><a href="#vehicles">Transport</a></li>
                    <li><a href="#culture">Culture</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <li><a href="#plan" class="btn" style="padding: 8px 20px; margin-top: -5px;">Plan Your Journey</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Discover the Last Shangri-La</h1>
                <p>Experience the magic of Bhutan with our authentic travel packages. From majestic dzongs to breathtaking Himalayan treks, we offer unforgettable journeys to the Land of the Thunder Dragon.</p>
                
                <div class="bhutan-flag">
                    <div class="flag-part flag-orange"></div>
                    <div class="flag-dragon"><i class="fas fa-dragon"></i></div>
                    <div class="flag-part flag-yellow"></div>
                </div>
                
                <a href="#plan" class="btn">Plan Your Bhutan Journey</a>
                
                <div class="visa-info">
                    <h4><i class="fas fa-passport"></i> Bhutan Visa Information</h4>
                    <p>All tourists (except Indian, Bangladeshi and Maldivian passport holders) require a visa to enter Bhutan. We handle the complete visa process for you!</p>
                    <p style="font-size: 0.9rem; margin-top: 10px;"><i class="fas fa-info-circle"></i> Minimum Daily Package: $250 per person in high season</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Plan Your Bhutan Journey Form -->
    <section id="plan">
        <div class="container">
            <div class="section-title">
                <h2>Plan Your Bhutan Journey</h2>
                <p>Fill out this form to get a personalized Bhutan travel itinerary and quote</p>
            </div>
            
            <div class="booking-form-container">
                <div class="form-header">
                    <h3><i class="fas fa-map-marked-alt"></i> Bhutan Travel Planner</h3>
                    <p>Complete this 4-step form to create your perfect Bhutan itinerary</p>
                </div>
                
                <!-- Form Progress -->
                <div class="form-progress">
                    <div class="progress-step active" id="step1">
                        <div class="step-number">1</div>
                        <div class="step-label">Basic Info</div>
                    </div>
                    <div class="progress-step" id="step2">
                        <div class="step-number">2</div>
                        <div class="step-label">Travel Details</div>
                    </div>
                    <div class="progress-step" id="step3">
                        <div class="step-number">3</div>
                        <div class="step-label">Activities</div>
                    </div>
                    <div class="progress-step" id="step4">
                        <div class="step-number">4</div>
                        <div class="step-label">Review</div>
                    </div>
                </div>
                
                <!-- Step 1: Basic Information -->
                <div class="form-step active" id="step1Form">
                    <h4><i class="fas fa-user-circle"></i> Traveler Information</h4>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <label for="fullName"><i class="fas fa-user"></i> Full Name</label>
                            <input type="text" id="fullName" class="form-control" placeholder="Enter your full name" required>
                            <div class="error-message" id="nameError">Please enter your full name</div>
                        </div>
                        <div class="form-group">
                            <label for="email"><i class="fas fa-envelope"></i> Email Address</label>
                            <input type="email" id="email" class="form-control" placeholder="your.email@example.com" required>
                            <div class="error-message" id="emailError">Please enter a valid email address</div>
                        </div>
                    </div>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <label for="phone"><i class="fas fa-phone"></i> Phone Number</label>
                            <input type="tel" id="phone" class="form-control" placeholder="+975 XXX XXX" required>
                        </div>
                        <div class="form-group">
                            <label for="country"><i class="fas fa-globe"></i> Country of Residence</label>
                            <select id="country" class="form-control" required>
                                <option value="">Select your country</option>
                                <option value="us">United States</option>
                                <option value="uk">United Kingdom</option>
                                <option value="aus">Australia</option>
                                <option value="can">Canada</option>
                                <option value="eu">European Union</option>
                                <option value="ind">India</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                    </div>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <label for="travelers"><i class="fas fa-users"></i> Number of Travelers</label>
                            <input type="number" id="travelers" class="form-control" min="1" max="20" value="2" required>
                        </div>
                        <div class="form-group">
                            <label for="travelMonth"><i class="fas fa-calendar-alt"></i> Preferred Travel Month</label>
                            <select id="travelMonth" class="form-control" required>
                                <option value="">Select month</option>
                                <option value="jan">January</option>
                                <option value="feb">February</option>
                                <option value="mar">March</option>
                                <option value="apr">April</option>
                                <option value="may">May</option>
                                <option value="jun">June</option>
                                <option value="jul">July</option>
                                <option value="aug">August</option>
                                <option value="sep">September</option>
                                <option value="oct">October</option>
                                <option value="nov">November</option>
                                <option value="dec">December</option>
                            </select>
                        </div>
                    </div>
                    
                    <div class="form-note">
                        <i class="fas fa-info-circle"></i> Your information is secure and will only be used to create your personalized Bhutan travel plan.
                    </div>
                    
                    <div class="form-actions">
                        <div></div>
                        <button type="button" class="btn" id="nextToStep2">Next <i class="fas fa-arrow-right"></i></button>
                    </div>
                </div>
                
                <!-- Step 2: Travel Details -->
                <div class="form-step" id="step2Form">
                    <h4><i class="fas fa-suitcase"></i> Travel Preferences</h4>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <label for="tourType"><i class="fas fa-map"></i> Tour Type</label>
                            <select id="tourType" class="form-control" required>
                                <option value="">Select tour type</option>
                                <option value="cultural">Cultural Tour</option>
                                <option value="trekking">Trekking Tour</option>
                                <option value="festival">Festival Tour</option>
                                <option value="honeymoon">Honeymoon Special</option>
                                <option value="wellness">Wellness & Meditation</option>
                                <option value="photography">Photography Tour</option>
                                <option value="custom">Custom Itinerary</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="duration"><i class="far fa-calendar-alt"></i> Duration (Days)</label>
                            <select id="duration" class="form-control" required>
                                <option value="5">5 Days</option>
                                <option value="7" selected>7 Days</option>
                                <option value="10">10 Days</option>
                                <option value="14">14 Days</option>
                                <option value="21">21 Days</option>
                            </select>
                        </div>
                    </div>
                    
                    <div class="form-row">
                        <div class="form-group">
                            <label for="accommodation"><i class="fas fa-hotel"></i> Accommodation Type</label>
                            <select id="accommodation" class="form-control" required>
                                <option value="standard">3-Star Standard</option>
                                <option value="firstclass" selected>4-Star First Class</option>
                                <option value="luxury">5-Star Luxury</option>
                                <option value="boutique">Boutique Hotels</option>
                                <option value="farmstay">Farm Stays</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="budget"><i class="fas fa-wallet"></i> Budget Per Person</label>
                            <select id="budget" class="form-control" required>
                                <option value="economy">Economy ($200-300/day)</option>
                                <option value="standard" selected>Standard ($300-400/day)</option>
                                <option value="premium">Premium ($400-500/day)</option>
                                <option value="luxury">Luxury ($500+/day)</option>
                            </select>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="destinations"><i class="fas fa-map-marker-alt"></i> Places You Want to Visit</label>
                        <textarea id="destinations" class="form-control" rows="3" placeholder="e.g., Paro, Thimphu, Punakha, Tiger's Nest Monastery..."></textarea>
                    </div>
                    
                    <div class="form-note">
                        <i class="fas fa-lightbulb"></i> Not sure what to choose? Our Bhutan experts can help you create the perfect itinerary based on your interests.
                    </div>
                    
                    <div class="form-actions">
                        <button type="button" class="btn btn-secondary" id="backToStep1"><i class="fas fa-arrow-left"></i> Back</button>
                        <button type="button" class="btn" id="nextToStep3">Next <i class="fas fa-arrow-right"></i></button>
                    </div>
                </div>
                
                <!-- Step 3: Activities & Transport -->
                <div class="form-step" id="step3Form">
                    <h4><i class="fas fa-hiking"></i> Activities & Transportation</h4>
                    
                    <div class="form-group">
                        <label><i class="fas fa-star"></i> Select Your Interests</label>
                        <div style="display: grid; grid-template-columns: repeat(auto-fill, minmax(200px, 1fr)); gap: 15px; margin-top: 10px;">
                            <label style="display: flex; align-items: center; cursor: pointer;">
                                <input type="checkbox" class="interest" value="monasteries" checked style="margin-right: 10px;">
                                Monasteries & Temples
                            </label>
                            <label style="display: flex; align-items: center; cursor: pointer;">
                                <input type="checkbox" class="interest" value="trekking" style="margin-right: 10px;">
                                Trekking & Hiking
                            </label>
                            <label style="display: flex; align-items: center; cursor: pointer;">
                                <input type="checkbox" class="interest" value="festivals" style="margin-right: 10px;">
                                Festivals & Culture
                            </label>
                            <label style="display: flex; align-items: center; cursor: pointer;">
                                <input type="checkbox" class="interest" value="wildlife" style="margin-right: 10px;">
                                Wildlife & Nature
                            </label>
                            <label style="display: flex; align-items: center; cursor: pointer;">
                                <input type="checkbox" class="interest" value="photography" style="margin-right: 10px;">
                                Photography
                            </label>
                            <label style="display: flex; align-items: center; cursor: pointer;">
                                <input type="checkbox" class="interest" value="meditation" style="margin-right: 10px;">
                                Meditation & Wellness
                            </label>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="vehicleType"><i class="fas fa-car"></i> Vehicle Preference</label>
                        <select id="vehicleType" class="form-control" required>
                            <option value="">Select vehicle type</option>
                            <option value="suv">SUV (1-4 people)</option>
                            <option value="van">Van (5-8 people)</option>
                            <option value="bus">Mini Bus (9-16 people)</option>
                            <option value="luxury">Luxury Vehicle</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="specialRequests"><i class="fas fa-comment-alt"></i> Special Requests</label>
                        <textarea id="specialRequests" class="form-control" rows="4" placeholder="Dietary requirements, special occasions, accessibility needs, or any other requests..."></textarea>
                    </div>
                    
                    <div class="form-note">
                        <i class="fas fa-car"></i> All our vehicles come with experienced Bhutanese drivers who know the roads and can share local insights.
                    </div>
                    
                    <div class="form-actions">
                        <button type="button" class="btn btn-secondary" id="backToStep2"><i class="fas fa-arrow-left"></i> Back</button>
                        <button type="button" class="btn" id="nextToStep4">Next <i class="fas fa-arrow-right"></i></button>
                    </div>
                </div>
                
                <!-- Step 4: Review & Submit -->
                <div class="form-step" id="step4Form">
                    <h4><i class="fas fa-clipboard-check"></i> Review Your Bhutan Journey Plan</h4>
                    
                    <div class="booking-summary" id="journeySummary">
                        <!-- Summary will be populated by JavaScript -->
                    </div>
                    
                    <div class="form-group">
                        <label for="howFound"><i class="fas fa-search"></i> How did you hear about us?</label>
                        <select id="howFound" class="form-control">
                            <option value="">Select option</option>
                            <option value="google">Google Search</option>
                            <option value="social">Social Media</option>
                            <option value="friend">Friend/Family Recommendation</option>
                            <option value="blog">Travel Blog</option>
                            <option value="other">Other</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label style="display: flex; align-items: flex-start; cursor: pointer;">
                            <input type="checkbox" id="terms" required style="margin-right: 10px; margin-top: 3px;">
                            <span>I agree to the <a href="#" style="color: var(--primary-color);">terms and conditions</a> and understand that a 20% deposit is required to confirm my Bhutan tour booking. I also understand that Bhutan visa processing will begin after deposit payment.</span>
                        </label>
                        <div class="error-message" id="termsError">You must agree to the terms and conditions</div>
                    </div>
                    
                    <div class="form-note">
                        <i class="fas fa-paper-plane"></i> After submitting, you'll receive a detailed itinerary and quote within 24 hours. One of our Bhutan travel experts will contact you to discuss your plan.
                    </div>
                    
                    <div class="form-actions">
                        <button type="button" class="btn btn-secondary" id="backToStep3"><i class="fas fa-arrow-left"></i> Back</button>
                        <button type="submit" class="btn" id="submitJourneyPlan"><i class="fas fa-paper-plane"></i> Submit Journey Plan</button>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Bhutan Tours Section -->
    <section id="tours">
        <div class="container">
            <div class="section-title">
                <h2>Bhutan Tour Packages</h2>
                <p>Discover our curated Bhutan experiences, from cultural immersions to spiritual journeys</p>
            </div>
            
            <div class="filters">
                <button class="filter-btn active" data-filter="all">All Tours</button>
                <button class="filter-btn" data-filter="cultural">Cultural</button>
                <button class="filter-btn" data-filter="trekking">Trekking</button>
                <button class="filter-btn" data-filter="festival">Festival</button>
                <button class="filter-btn" data-filter="luxury">Luxury</button>
            </div>
            
            <div class="tour-cards" id="tourCards">
                <!-- Tour cards will be populated by JavaScript -->
            </div>
        </div>
    </section>

    <!-- Trekking Packages -->
    <section id="trekking" class="trekking-packages">
        <div class="container">
            <div class="section-title">
                <h2>Bhutan Trekking Adventures</h2>
                <p>Experience the Himalayas with our guided treks to some of Bhutan's most spectacular regions</p>
            </div>
            
            <div class="package-cards" id="trekkingCards">
                <!-- Trekking packages will be populated by JavaScript -->
            </div>
        </div>
    </section>

    <!-- Enhanced Vehicle Rental Section -->
    <section id="vehicles" class="vehicle-section">
        <div class="container">
            <div class="section-title">
                <h2>Transportation in Bhutan</h2>
                <p>Choose from our fleet of comfortable vehicles with experienced Bhutanese drivers</p>
            </div>
            
            <div class="vehicle-filters">
                <button class="vehicle-filter-btn active" data-vehicle-filter="all">All Vehicles</button>
                <button class="vehicle-filter-btn" data-vehicle-filter="suv">SUVs</button>
                <button class="vehicle-filter-btn" data-vehicle-filter="van">Vans</button>
                <button class="vehicle-filter-btn" data-vehicle-filter="luxury">Luxury</button>
                <button class="vehicle-filter-btn" data-vehicle-filter="bus">Buses</button>
            </div>
            
            <div class="vehicle-cards" id="vehicleCards">
                <!-- Vehicle cards will be populated by JavaScript -->
            </div>
            
            <div style="text-align: center; margin-top: 30px;">
                <a href="#plan" class="btn"><i class="fas fa-car"></i> Book Vehicle in Your Journey Plan</a>
            </div>
        </div>
    </section>

    <!-- Cultural Experiences -->
    <section id="culture" class="bhutan-special">
        <div class="container">
            <div class="section-title">
                <h2>Bhutan Cultural Experiences</h2>
                <p>Immerse yourself in Bhutan's unique traditions and way of life</p>
            </div>
            
            <div class="culture-cards">
                <div class="culture-card">
                    <div class="culture-icon">
                        <i class="fas fa-landmark"></i>
                    </div>
                    <h3>Dzong Visits</h3>
                    <p>Explore magnificent fortress-monasteries like Punakha Dzong and Paro Dzong</p>
                </div>
                
                <div class="culture-card">
                    <div class="culture-icon">
                        <i class="fas fa-mask"></i>
                    </div>
                    <h3>Festival Tours</h3>
                    <p>Witness colorful Tshechu festivals with mask dances and religious ceremonies</p>
                </div>
                
                <div class="culture-card">
                    <div class="culture-icon">
                        <i class="fas fa-hiking"></i>
                    </div>
                    <h3>Tiger's Nest Trek</h3>
                    <p>Hike to the iconic Taktsang Monastery, perched on a cliff 900m above Paro Valley</p>
                </div>
                
                <div class="culture-card">
                    <div class="culture-icon">
                        <i class="fas fa-utensils"></i>
                    </div>
                    <h3>Bhutanese Cuisine</h3>
                    <p>Traditional cooking classes and meals with local families</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Contact Our Bhutan Experts</h2>
                <p>Get in touch with our team for personalized Bhutan travel planning</p>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <div>
                            <h3>Our Offices</h3>
                            <p>Thimphu, Bhutan (Head Office)</p>
                            <p>Paro, Bhutan (Tour Operations)</p>
                            <p>Delhi, India (Regional Office)</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-phone"></i>
                        </div>
                        <div>
                            <h3>Phone Numbers</h3>
                            <p>Bhutan: +975-17-123-456</p>
                            <p>India: +91-11-2345-6789</p>
                            <p>International: +1-800-BHUTAN</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div>
                            <h3>Email Address</h3>
                            <p>info@drukjourney.com</p>
                            <p>bookings@drukjourney.com</p>
                            <p>visa@drukjourney.com</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-clock"></i>
                        </div>
                        <div>
                            <h3>Operating Hours</h3>
                            <p>Bhutan Time (GMT+6)</p>
                            <p>Mon-Fri: 9:00 AM - 6:00 PM</p>
                            <p>Sat: 10:00 AM - 4:00 PM</p>
                        </div>
                    </div>
                </div>
                
                <div class="contact-form">
                    <h3>Send us a Message</h3>
                    <form id="contactForm">
                        <div class="form-row">
                            <div class="form-group">
                                <label for="contactName">Full Name</label>
                                <input type="text" id="contactName" class="form-control" placeholder="Your Name" required>
                            </div>
                            <div class="form-group">
                                <label for="contactEmail">Email Address</label>
                                <input type="email" id="contactEmail" class="form-control" placeholder="Your Email" required>
                            </div>
                        </div>
                        
                        <div class="form-group">
                            <label for="contactSubject">Subject</label>
                            <input type="text" id="contactSubject" class="form-control" placeholder="Subject" required>
                        </div>
                        
                        <div class="form-group">
                            <label for="contactMessage">Message</label>
                            <textarea id="contactMessage" class="form-control" rows="5" placeholder="Your message..." required></textarea>
                        </div>
                        
                        <button type="submit" class="btn">Send Message</button>
                    </form>
                </div>
            </div>
            
            <div class="map-container">
                <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d113446.96577612106!2d89.58615023299638!3d27.472782850417893!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x39e194199620d8c7%3A0x5b6392b8a8c33d3c!2sThimphu%2C%20Bhutan!5e0!3m2!1sen!2s!4v1686754438616!5m2!1sen!2s" allowfullscreen="" loading="lazy"></iframe>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-about">
                    <div class="footer-logo"><i class="fas fa-dragon"></i> Druk Journey</div>
                    <p>Official Bhutan Tour Operator licensed by the Tourism Council of Bhutan. We specialize in authentic, sustainable travel experiences in the Land of the Thunder Dragon.</p>
                    <div class="social-icons">
                        <a href="#" class="social-icon"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-instagram"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-youtube"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-whatsapp"></i></a>
                    </div>
                </div>
                
                <div class="footer-links">
                    <h3>Quick Links</h3>
                    <ul>
                        <li><a href="#home">Home</a></li>
                        <li><a href="#tours">Bhutan Tours</a></li>
                        <li><a href="#trekking">Trekking</a></li>
                        <li><a href="#vehicles">Transport</a></li>
                        <li><a href="#culture">Culture</a></li>
                        <li><a href="#plan">Plan Your Journey</a></li>
                    </ul>
                </div>
                
                <div class="footer-newsletter">
                    <h3>Bhutan Travel Updates</h3>
                    <p>Subscribe for Bhutan travel news, festival dates, and special offers</p>
                    <form class="newsletter-form" id="newsletterForm">
                        <input type="email" class="form-control" placeholder="Your Email Address" required>
                        <button type="submit" class="btn">Subscribe</button>
                    </form>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2023 Druk Journey Bhutan Travel Specialists. All rights reserved. | Licensed by Tourism Council of Bhutan | GSTN: BTN-123456789</p>
            </div>
        </div>
    </footer>

    <!-- Enhanced Chat Bot -->
    <div class="chatbot-container">
        <div class="chatbot-toggle" id="chatbotToggle">
            <i class="fas fa-comments"></i>
        </div>
        <div class="chatbot-window" id="chatbotWindow">
            <div class="chatbot-header">
                <h3><i class="fas fa-dragon"></i> Druk Journey Assistant</h3>
                <button class="chatbot-close" id="chatbotClose">&times;</button>
            </div>
            <div class="chatbot-messages" id="chatbotMessages">
                <div class="message bot-message">
                    <strong>Tashi Delek!</strong> Welcome to Druk Journey. I'm here to help you plan your Bhutan adventure. How can I assist you today?
                </div>
                <div class="message bot-message">
                    <strong>Quick questions you can ask:</strong>
                    <div class="quick-replies">
                        <div class="quick-reply" data-reply="Bhutan visa">Bhutan visa</div>
                        <div class="quick-reply" data-reply="Tour packages">Tour packages</div>
                        <div class="quick-reply" data-reply="Best time to visit">Best time</div>
                        <div class="quick-reply" data-reply="Festival dates">Festivals</div>
                    </div>
                </div>
            </div>
            <div class="chatbot-input">
                <input type="text" id="chatInput" placeholder="Ask about Bhutan travel...">
                <button id="sendChat"><i class="fas fa-paper-plane"></i></button>
            </div>
        </div>
    </div>

    <!-- Journey Plan Success Modal -->
    <div class="modal" id="successModal">
        <div class="modal-content">
            <button class="modal-close" id="successModalClose">&times;</button>
            <div style="text-align: center; padding: 20px;">
                <div style="font-size: 4rem; color: var(--primary-color); margin-bottom: 20px;">
                    <i class="fas fa-check-circle"></i>
                </div>
                <h3>Journey Plan Submitted!</h3>
                <p>Thank you for planning your Bhutan journey with us. We've received your travel preferences and will contact you within 24 hours with a detailed itinerary and quote.</p>
                
                <div style="background-color: #f9f9f9; padding: 20px; border-radius: var(--border-radius); margin: 25px 0; text-align: left;">
                    <h4>What happens next?</h4>
                    <ul style="margin-left: 20px; margin-top: 10px;">
                        <li>1. Our Bhutan expert will review your preferences</li>
                        <li>2. You'll receive a customized itinerary & quote</li>
                        <li>3. We'll schedule a call to discuss your plan</li>
                        <li>4. Once confirmed, we'll start visa processing</li>
                    </ul>
                </div>
                
                <p><strong>Reference ID:</strong> <span id="referenceId" style="color: var(--primary-color); font-weight: 600;">DJ-2023-001</span></p>
                
                <button class="btn" id="closeSuccessModal" style="margin-top: 20px; width: 100%;">Continue Exploring</button>
            </div>
        </div>
    </div>

    <!-- Vehicle Booking Modal -->
    <div class="modal" id="vehicleModal">
        <div class="modal-content">
            <button class="modal-close" id="vehicleModalClose">&times;</button>
            <h3><i class="fas fa-car"></i> Book Vehicle</h3>
            <div id="vehicleModalContent">
                <!-- Vehicle booking form will be populated by JavaScript -->
            </div>
        </div>
    </div>

    <script>
        // Main JavaScript for Bhutan Travel Agency Website
        
        // DOM Elements
        const hamburger = document.getElementById('hamburger');
        const navLinks = document.getElementById('navLinks');
        const navItems = document.querySelectorAll('.nav-links a');
        const journeySummary = document.getElementById('journeySummary');
        
        // Form Elements
        const step1Form = document.getElementById('step1Form');
        const step2Form = document.getElementById('step2Form');
        const step3Form = document.getElementById('step3Form');
        const step4Form = document.getElementById('step4Form');
        
        const step1 = document.getElementById('step1');
        const step2 = document.getElementById('step2');
        const step3 = document.getElementById('step3');
        const step4 = document.getElementById('step4');
        
        const nextToStep2 = document.getElementById('nextToStep2');
        const nextToStep3 = document.getElementById('nextToStep3');
        const nextToStep4 = document.getElementById('nextToStep4');
        
        const backToStep1 = document.getElementById('backToStep1');
        const backToStep2 = document.getElementById('backToStep2');
        const backToStep3 = document.getElementById('backToStep3');
        
        const submitJourneyPlan = document.getElementById('submitJourneyPlan');
        
        // Tour Elements
        const tourCardsContainer = document.getElementById('tourCards');
        const trekkingCardsContainer = document.getElementById('trekkingCards');
        const vehicleCardsContainer = document.getElementById('vehicleCards');
        const filterButtons = document.querySelectorAll('.filter-btn');
        const vehicleFilterButtons = document.querySelectorAll('.vehicle-filter-btn');
        
        // Modal Elements
        const successModal = document.getElementById('successModal');
        const successModalClose = document.getElementById('successModalClose');
        const closeSuccessModal = document.getElementById('closeSuccessModal');
        const vehicleModal = document.getElementById('vehicleModal');
        const vehicleModalClose = document.getElementById('vehicleModalClose');
        
        // Chat Bot Elements
        const chatbotToggle = document.getElementById('chatbotToggle');
        const chatbotWindow = document.getElementById('chatbotWindow');
        const chatbotClose = document.getElementById('chatbotClose');
        const chatbotMessages = document.getElementById('chatbotMessages');
        const chatInput = document.getElementById('chatInput');
        const sendChat = document.getElementById('sendChat');

        // Bhutan Travel Data
        const bhutanTours = [
            { id: 1, name: "Classic Bhutan Cultural Tour", type: "cultural", price: 1750, duration: 7, rating: 4.9, image: "https://images.unsplash.com/photo-1580737661251-9d1c8543b0c4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "Explore Thimphu, Punakha, and Paro with visits to iconic dzongs and monasteries.", highlights: ["Punakha Dzong", "Tiger's Nest Monastery", "Buddha Dordenma"] },
            { id: 2, name: "Druk Path Trek", type: "trekking", price: 2200, duration: 10, rating: 4.8, image: "https://images.unsplash.com/photo-1551632811-561732d1e306?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "Moderate trek from Paro to Thimphu with stunning Himalayan views and lake visits.", highlights: ["Jili Dzong", "Jangchulakha", "Jimilang Tsho Lake"] },
            { id: 3, name: "Bhutan Festival Tour", type: "festival", price: 1950, duration: 8, rating: 4.9, image: "https://images.unsplash.com/photo-1548013146-72479768bada?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "Experience vibrant Paro or Thimphu Tshechu festivals with mask dances.", highlights: ["Festival Mask Dances", "Sacred Relic Display", "Local Celebrations"] },
            { id: 4, name: "Luxury Bhutan Honeymoon", type: "luxury", price: 3200, duration: 9, rating: 5.0, image: "https://images.unsplash.com/photo-1520250497591-112f2f40a3f4?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "Romantic getaway with luxury resorts, private tours, and special experiences.", highlights: ["Luxury Resort Stays", "Private Guide", "Romantic Dinners"] },
            { id: 5, name: "Bhutan Spiritual Journey", type: "cultural", price: 1850, duration: 8, rating: 4.7, image: "https://images.unsplash.com/photo-1544551763-46a013bb70d5?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "Meditation, monastery visits, and meetings with Buddhist monks.", highlights: ["Meditation Sessions", "Monastery Stays", "Monk Teachings"] },
            { id: 6, name: "Birdwatching in Bhutan", type: "cultural", price: 1650, duration: 7, rating: 4.6, image: "https://images.unsplash.com/photo-1551085254-e96b210db58a?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "For nature enthusiasts with expert guides to spot rare Himalayan birds.", highlights: ["Expert Bird Guide", "Protected Areas", "Rare Species"] }
        ];

        const trekkingPackages = [
            { id: 1, name: "Jomolhari Trek", difficulty: "Strenuous", duration: "9 days", price: 2500, image: "https://images.unsplash.com/photo-1551632811-561732d1e306?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "Trek to the base of Mount Jomolhari (7,326m) with spectacular mountain views." },
            { id: 2, name: "Dagala Thousand Lakes", difficulty: "Moderate", duration: "6 days", price: 1800, image: "https://images.unsplash.com/photo-1501554728187-ce583db33af7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "Pass through beautiful alpine lakes with chances to spot high-altitude wildlife." },
            { id: 3, name: "Bumthang Cultural Trek", difficulty: "Easy", duration: "4 days", price: 1200, image: "https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1770&q=80", description: "Gentle trek through Bumthang Valley with visits to ancient temples and villages." }
        ];

        // Enhanced Vehicle Data
        const vehicles = [
            { id: 1, name: "Toyota Land Cruiser", type: "suv", category: "suv", price: 120, image: "https://images.unsplash.com/photo-1544636331-e26879cd4d9b?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80", capacity: "Up to 4 passengers", features: ["4WD", "Air Conditioning", "Experienced Driver", "Luggage Space"], description: "Perfect for mountainous terrain and small groups." },
            { id: 2, name: "Toyota Fortuner", type: "suv", category: "suv", price: 100, image: "https://images.unsplash.com/photo-1553440569-bcc63803a83d?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1325&q=80", capacity: "Up to 5 passengers", features: ["Comfortable Seating", "AC", "Bluetooth", "Spacious"], description: "Reliable SUV for family trips across Bhutan." },
            { id: 3, name: "Toyota Hiace Van", type: "van", category: "van", price: 150, image: "https://images.unsplash.com/photo-1568605114967-8130f3a36994?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80", capacity: "Up to 8 passengers", features: ["Spacious Interior", "AC", "Comfortable for Groups", "Luggage Rack"], description: "Ideal for larger groups or families traveling together." },
            { id: 4, name: "Hyundai Staria Luxury", type: "van", category: "luxury", price: 200, image: "https://images.unsplash.com/photo-1549399542-7e3f8b79c341?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80", capacity: "Up to 7 passengers", features: ["Premium Interior", "WiFi", "Entertainment System", "Refreshments"], description: "Luxury travel experience with premium amenities." },
            { id: 5, name: "Mercedes Benz V-Class", type: "van", category: "luxury", price: 250, image: "https://images.unsplash.com/photo-1563720223485-8d6d5c57d5f7?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80", capacity: "Up to 6 passengers", features: ["Executive Seats", "Privacy Glass", "Premium Sound", "Chauffeur"], description: "Ultimate luxury transport for discerning travelers." },
            { id: 6, name: "Mini Bus 16-Seater", type: "bus", category: "bus", price: 300, image: "https://images.unsplash.com/photo-1590490360182-c33d57733427?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1374&q=80", capacity: "Up to 16 passengers", features: ["Comfortable Seating", "AC", "PA System", "Luggage Compartment"], description: "Perfect for large groups, corporate tours, or family reunions." },
            { id: 7, name: "Honda City Sedan", type: "suv", category: "suv", price: 80, image: "https://images.unsplash.com/photo-1549317661-bd32c8ce0db2?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80", capacity: "Up to 3 passengers", features: ["Fuel Efficient", "AC", "Economical", "Compact"], description: "Budget-friendly option for solo travelers or couples." },
            { id: 8, name: "Toyota Coaster Bus", type: "bus", category: "bus", price: 350, image: "https://images.unsplash.com/photo-1558618666-fcd25c85cd64?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=1470&q=80", capacity: "Up to 24 passengers", features: ["Large Capacity", "AC", "Comfortable", "Tour Guide Seat"], description: "For large tour groups with ample space for luggage." }
        ];

        // Chat Bot Responses
        const chatBotResponses = {
            "greeting": ["Tashi Delek! Welcome to Druk Journey. How can I help you plan your Bhutan adventure today?", "Hello! I'm your Bhutan travel assistant. What would you like to know about traveling to Bhutan?"],
            "bhutan visa": ["All tourists (except Indian, Bangladeshi and Maldivian passport holders) require a visa to enter Bhutan. We handle the complete visa process for you after booking. The minimum daily package is $250 per person in high season (Mar-May, Sep-Nov) and $200 in low season (Jun-Aug, Dec-Feb)."],
            "tour packages": ["We offer various Bhutan tour packages: Cultural tours (7 days from $1750), Trekking adventures (10 days from $2200), Festival tours (8 days from $1950), and Luxury experiences (9 days from $3200). You can also customize your own itinerary."],
            "best time to visit": ["The best time to visit Bhutan is during spring (March to May) when flowers bloom and autumn (September to November) for clear mountain views and festivals. Summer (June to August) is monsoon season with lush landscapes, and winter (December to February) is cold but great for photography with snow-capped mountains."],
            "festival dates": ["Major Bhutan festivals (Tshechus) occur throughout the year! Paro Tshechu (spring), Thimphu Tshechu (autumn), and Punakha Tshechu (winter) are the most popular. Festival dates follow the lunar calendar, so they change each year. Would you like me to check specific festival dates for your travel period?"],
            "cost": ["Bhutan has a Minimum Daily Package fee: $250 per person per night in high season (Mar-May, Sep-Nov) and $200 in low season (Jun-Aug, Dec-Feb). This includes accommodation, all meals, transport, guide, and sustainable tourism royalty. Additional costs depend on your accommodation choice and activities."],
            "transport": ["We provide various vehicles: SUVs ($80-120/day), Vans ($150-200/day), Luxury vehicles ($200-250/day), and Buses ($300-350/day). All include experienced Bhutanese drivers. You can select your vehicle in the 'Plan Your Journey' form."],
            "trekking": ["Bhutan offers amazing treks for all levels: Druk Path Trek (moderate, 6-7 days), Jomolhari Trek (strenuous, 9 days), and Bumthang Cultural Trek (easy, 4 days). All treks include guides, camping equipment, cooks, and meals. We recommend trekking in spring or autumn."],
            "culture": ["Bhutanese culture is unique! Must-see experiences include visiting dzongs (fortress-monasteries), attending festivals with mask dances, hiking to Tiger's Nest Monastery, trying traditional cuisine like ema datshi (chili cheese), and learning about Gross National Happiness."],
            "accommodation": ["We offer various accommodations: 3-star standard hotels ($100-150/night), 4-star first class hotels ($150-250/night), 5-star luxury resorts ($250-400/night), and unique options like farm stays and boutique hotels. All are included in the daily package rate."],
            "plan": ["You can plan your Bhutan journey using our online form! Just click 'Plan Your Journey' in the navigation or scroll to the form section. It takes about 5 minutes to complete, and our experts will create a personalized itinerary for you."],
            "contact": ["You can contact us at info@drukjourney.com or call +975-17-123-456 (Bhutan) / +91-11-2345-6789 (India). Our offices are in Thimphu, Paro, and Delhi. We're available Monday-Friday 9AM-6PM Bhutan time."],
            "default": ["I'm not sure about that. Would you like to know about Bhutan visas, tour packages, the best time to visit, or festival dates? You can also use the 'Plan Your Journey' form to get a personalized itinerary."]
        };

        // Initialize the website
        document.addEventListener('DOMContentLoaded', function() {
            // Initialize components
            initNavbar();
            initForm();
            initTourFiltering();
            initVehicleFiltering();
            populateTourCards();
            populateTrekkingCards();
            populateVehicleCards();
            setupChatBot();
            
            // Set active nav item based on scroll position
            window.addEventListener('scroll', setActiveNavItem);
            
            // Check for stored journey plans
            const storedPlan = localStorage.getItem('bhutanJourneyPlan');
            if (storedPlan) {
                console.log('Previous journey plan found:', JSON.parse(storedPlan));
            }
        });

        // Initialize navbar functionality
        function initNavbar() {
            hamburger.addEventListener('click', function() {
                navLinks.classList.toggle('active');
                hamburger.innerHTML = navLinks.classList.contains('active') ? 
                    '<i class="fas fa-times"></i>' : '<i class="fas fa-bars"></i>';
            });

            // Close mobile menu when clicking on a link
            navItems.forEach(item => {
                item.addEventListener('click', function() {
                    if (window.innerWidth <= 768) {
                        navLinks.classList.remove('active');
                        hamburger.innerHTML = '<i class="fas fa-bars"></i>';
                    }
                });
            });
        }

        // Initialize multi-step form
        function initForm() {
            // Step navigation
            nextToStep2.addEventListener('click', function() {
                if (validateStep1()) {
                    goToStep(2);
                    updateProgress(2);
                }
            });
            
            nextToStep3.addEventListener('click', function() {
                if (validateStep2()) {
                    goToStep(3);
                    updateProgress(3);
                }
            });
            
            nextToStep4.addEventListener('click', function() {
                if (validateStep3()) {
                    goToStep(4);
                    updateProgress(4);
                    updateJourneySummary();
                }
            });
            
            backToStep1.addEventListener('click', function() {
                goToStep(1);
                updateProgress(1);
            });
            
            backToStep2.addEventListener('click', function() {
                goToStep(2);
                updateProgress(2);
            });
            
            backToStep3.addEventListener('click', function() {
                goToStep(3);
                updateProgress(3);
            });
            
            // Form submission
            submitJourneyPlan.addEventListener('click', function(e) {
                e.preventDefault();
                if (validateStep4()) {
                    submitJourneyPlanToServer();
                }
            });
            
            // Modal close buttons
            successModalClose.addEventListener('click', function() {
                successModal.style.display = 'none';
            });
            
            closeSuccessModal.addEventListener('click', function() {
                successModal.style.display = 'none';
            });
            
            vehicleModalClose.addEventListener('click', function() {
                vehicleModal.style.display = 'none';
            });
            
            // Close modals when clicking outside
            window.addEventListener('click', function(event) {
                if (event.target === successModal) {
                    successModal.style.display = 'none';
                }
                if (event.target === vehicleModal) {
                    vehicleModal.style.display = 'none';
                }
            });
        }

        // Form validation functions
        function validateStep1() {
            const fullName = document.getElementById('fullName').value;
            const email = document.getElementById('email').value;
            const country = document.getElementById('country').value;
            
            let isValid = true;
            
            // Reset errors
            document.getElementById('nameError').style.display = 'none';
            document.getElementById('emailError').style.display = 'none';
            
            // Validate name
            if (fullName.trim() === '') {
                document.getElementById('nameError').style.display = 'block';
                isValid = false;
            }
            
            // Validate email
            const emailPattern = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
            if (!emailPattern.test(email)) {
                document.getElementById('emailError').style.display = 'block';
                isValid = false;
            }
            
            // Validate country
            if (country === '') {
                alert('Please select your country of residence');
                isValid = false;
            }
            
            return isValid;
        }

        function validateStep2() {
            const tourType = document.getElementById('tourType').value;
            const duration = document.getElementById('duration').value;
            
            if (tourType === '') {
                alert('Please select a tour type');
                return false;
            }
            
            if (duration === '') {
                alert('Please select a duration');
                return false;
            }
            
            return true;
        }

        function validateStep3() {
            const vehicleType = document.getElementById('vehicleType').value;
            
            if (vehicleType === '') {
                alert('Please select a vehicle type');
                return false;
            }
            
            return true;
        }

        function validateStep4() {
            const terms = document.getElementById('terms').checked;
            
            if (!terms) {
                document.getElementById('termsError').style.display = 'block';
                return false;
            }
            
            document.getElementById('termsError').style.display = 'none';
            return true;
        }

        // Form navigation
        function goToStep(stepNumber) {
            // Hide all steps
            step1Form.classList.remove('active');
            step2Form.classList.remove('active');
            step3Form.classList.remove('active');
            step4Form.classList.remove('active');
            
            // Show selected step
            document.getElementById(`step${stepNumber}Form`).classList.add('active');
        }

        function updateProgress(stepNumber) {
            // Reset all steps
            step1.classList.remove('active', 'completed');
            step2.classList.remove('active', 'completed');
            step3.classList.remove('active', 'completed');
            step4.classList.remove('active', 'completed');
            
            // Update steps based on current step
            for (let i = 1; i <= 4; i++) {
                const stepElement = document.getElementById(`step${i}`);
                if (i < stepNumber) {
                    stepElement.classList.add('completed');
                } else if (i === stepNumber) {
                    stepElement.classList.add('active');
                }
            }
        }

        // Update journey summary
        function updateJourneySummary() {
            const fullName = document.getElementById('fullName').value;
            const email = document.getElementById('email').value;
            const country = document.getElementById('country').value;
            const travelers = document.getElementById('travelers').value;
            const travelMonth = document.getElementById('travelMonth').value;
            const tourType = document.getElementById('tourType').value;
            const duration = document.getElementById('duration').value;
            const accommodation = document.getElementById('accommodation').value;
            const budget = document.getElementById('budget').value;
            const destinations = document.getElementById('destinations').value;
            const vehicleType = document.getElementById('vehicleType').value;
            const specialRequests = document.getElementById('specialRequests').value;
            
            // Get selected interests
            const interestCheckboxes = document.querySelectorAll('.interest:checked');
            const interests = Array.from(interestCheckboxes).map(cb => {
                const value = cb.value;
                return value.charAt(0).toUpperCase() + value.slice(1);
            }).join(', ');
            
            // Format month
            const monthNames = {
                'jan': 'January', 'feb': 'February', 'mar': 'March', 'apr': 'April',
                'may': 'May', 'jun': 'June', 'jul': 'July', 'aug': 'August',
                'sep': 'September', 'oct': 'October', 'nov': 'November', 'dec': 'December'
            };
            
            // Format tour type
            const tourTypeNames = {
                'cultural': 'Cultural Tour',
                'trekking': 'Trekking Tour',
                'festival': 'Festival Tour',
                'honeymoon': 'Honeymoon Special',
                'wellness': 'Wellness & Meditation',
                'photography': 'Photography Tour',
                'custom': 'Custom Itinerary'
            };
            
            // Format accommodation
            const accommodationNames = {
                'standard': '3-Star Standard',
                'firstclass': '4-Star First Class',
                'luxury': '5-Star Luxury',
                'boutique': 'Boutique Hotels',
                'farmstay': 'Farm Stays'
            };
            
            // Format budget
            const budgetNames = {
                'economy': 'Economy ($200-300/day)',
                'standard': 'Standard ($300-400/day)',
                'premium': 'Premium ($400-500/day)',
                'luxury': 'Luxury ($500+/day)'
            };
            
            // Format vehicle
            const vehicleNames = {
                'suv': 'SUV (1-4 people)',
                'van': 'Van (5-8 people)',
                'bus': 'Mini Bus (9-16 people)',
                'luxury': 'Luxury Vehicle'
            };
            
            // Create summary HTML
            journeySummary.innerHTML = `
                <div class="summary-item">
                    <span>Traveler Name</span>
                    <span>${fullName}</span>
                </div>
                <div class="summary-item">
                    <span>Email</span>
                    <span>${email}</span>
                </div>
                <div class="summary-item">
                    <span>Travelers</span>
                    <span>${travelers} person(s)</span>
                </div>
                <div class="summary-item">
                    <span>Travel Month</span>
                    <span>${monthNames[travelMonth] || travelMonth}</span>
                </div>
                <div class="summary-item">
                    <span>Tour Type</span>
                    <span>${tourTypeNames[tourType] || tourType}</span>
                </div>
                <div class="summary-item">
                    <span>Duration</span>
                    <span>${duration} days</span>
                </div>
                <div class="summary-item">
                    <span>Accommodation</span>
                    <span>${accommodationNames[accommodation] || accommodation}</span>
                </div>
                <div class="summary-item">
                    <span>Budget Level</span>
                    <span>${budgetNames[budget] || budget}</span>
                </div>
                <div class="summary-item">
                    <span>Vehicle Type</span>
                    <span>${vehicleNames[vehicleType] || vehicleType}</span>
                </div>
                ${destinations ? `
                <div class="summary-item">
                    <span>Destinations of Interest</span>
                    <span>${destinations}</span>
                </div>
                ` : ''}
                ${interests ? `
                <div class="summary-item">
                    <span>Interests</span>
                    <span>${interests}</span>
                </div>
                ` : ''}
                ${specialRequests ? `
                <div class="summary-item">
                    <span>Special Requests</span>
                    <span>${specialRequests}</span>
                </div>
                ` : ''}
            `;
        }

        // Submit journey plan
        function submitJourneyPlanToServer() {
            // Collect all form data
            const formData = {
                fullName: document.getElementById('fullName').value,
                email: document.getElementById('email').value,
                phone: document.getElementById('phone').value,
                country: document.getElementById('country').value,
                travelers: document.getElementById('travelers').value,
                travelMonth: document.getElementById('travelMonth').value,
                tourType: document.getElementById('tourType').value,
                duration: document.getElementById('duration').value,
                accommodation: document.getElementById('accommodation').value,
                budget: document.getElementById('budget').value,
                destinations: document.getElementById('destinations').value,
                vehicleType: document.getElementById('vehicleType').value,
                specialRequests: document.getElementById('specialRequests').value,
                howFound: document.getElementById('howFound').value,
                timestamp: new Date().toISOString()
            };
            
            // Get selected interests
            const interestCheckboxes = document.querySelectorAll('.interest:checked');
            formData.interests = Array.from(interestCheckboxes).map(cb => cb.value);
            
            // Store in localStorage (simulating server submission)
            localStorage.setItem('bhutanJourneyPlan', JSON.stringify(formData));
            
            // Generate reference ID
            const referenceId = 'DJ-' + new Date().getFullYear() + '-' + Math.floor(1000 + Math.random() * 9000);
            document.getElementById('referenceId').textContent = referenceId;
            
            // Show success modal
            successModal.style.display = 'flex';
            
            // Reset form after delay (optional)
            setTimeout(() => {
                // Reset to step 1
                goToStep(1);
                updateProgress(1);
                
                // Clear form (optional)
                // document.getElementById('bhutanBookingForm').reset();
            }, 3000);
        }

        // Initialize tour filtering
        function initTourFiltering() {
            filterButtons.forEach(button => {
                button.addEventListener('click', function() {
                    // Remove active class from all buttons
                    filterButtons.forEach(btn => btn.classList.remove('active'));
                    
                    // Add active class to clicked button
                    this.classList.add('active');
                    
                    // Get filter value
                    const filterValue = this.getAttribute('data-filter');
                    
                    // Filter tours
                    filterTours(filterValue);
                });
            });
        }

        // Initialize vehicle filtering
        function initVehicleFiltering() {
            vehicleFilterButtons.forEach(button => {
                button.addEventListener('click', function() {
                    // Remove active class from all buttons
                    vehicleFilterButtons.forEach(btn => btn.classList.remove('active'));
                    
                    // Add active class to clicked button
                    this.classList.add('active');
                    
                    // Get filter value
                    const filterValue = this.getAttribute('data-vehicle-filter');
                    
                    // Filter vehicles
                    filterVehicles(filterValue);
                });
            });
        }

        // Filter tours based on selected filter
        function filterTours(filter) {
            let filteredTours = bhutanTours;
            
            if (filter !== 'all') {
                filteredTours = bhutanTours.filter(tour => tour.type === filter);
            }
            
            populateTourCards(filteredTours);
        }

        // Filter vehicles based on selected filter
        function filterVehicles(filter) {
            let filteredVehicles = vehicles;
            
            if (filter !== 'all') {
                filteredVehicles = vehicles.filter(vehicle => vehicle.category === filter);
            }
            
            populateVehicleCards(filteredVehicles);
        }

        // Populate tour cards
        function populateTourCards(toursToShow = bhutanTours) {
            tourCardsContainer.innerHTML = '';
            
            toursToShow.forEach(tour => {
                const ratingStars = generateRatingStars(tour.rating);
                const highlightsHTML = tour.highlights.map(highlight => `<li><i class="fas fa-check"></i> ${highlight}</li>`).join('');
                
                const tourCard = document.createElement('div');
                tourCard.className = 'tour-card';
                tourCard.setAttribute('data-type', tour.type);
                
                tourCard.innerHTML = `
                    <div class="tour-img">
                        <img src="${tour.image}" alt="${tour.name}">
                    </div>
                    <div class="tour-content">
                        <div class="tour-header">
                            <h3>${tour.name}</h3>
                            <div class="tour-price">$${tour.price}</div>
                        </div>
                        <p>${tour.description}</p>
                        <div class="tour-duration">
                            <i class="far fa-calendar-alt"></i> ${tour.duration} Days
                        </div>
                        <ul style="margin: 10px 0 15px 15px; font-size: 0.9rem;">
                            ${highlightsHTML}
                        </ul>
                        <div class="tour-rating">
                            ${ratingStars}
                            <span>${tour.rating}/5</span>
                        </div>
                        <a href="#plan" class="btn" style="margin-top: 15px; width: 100%; display: block; text-align: center;">
                            Add to My Journey
                        </a>
                    </div>
                `;
                
                tourCardsContainer.appendChild(tourCard);
            });
        }

        // Populate trekking cards
        function populateTrekkingCards() {
            trekkingCardsContainer.innerHTML = '';
            
            trekkingPackages.forEach(trek => {
                const trekCard = document.createElement('div');
                trekCard.className = 'package-card';
                
                trekCard.innerHTML = `
                    <div class="tour-img">
                        <img src="${trek.image}" alt="${trek.name}">
                    </div>
                    <div class="tour-content">
                        <div class="tour-header">
                            <h3>${trek.name}</h3>
                            <div class="tour-price">$${trek.price}</div>
                        </div>
                        <p>${trek.description}</p>
                        <div class="tour-duration">
                            <i class="far fa-calendar-alt"></i> ${trek.duration}
                        </div>
                        <div class="difficulty">${trek.difficulty}</div>
                        <a href="#plan" class="btn" style="margin-top: 15px; width: 100%; display: block; text-align: center;">
                            Add to My Journey
                        </a>
                    </div>
                `;
                
                trekkingCardsContainer.appendChild(trekCard);
            });
        }

        // Populate vehicle cards
        function populateVehicleCards(vehiclesToShow = vehicles) {
            vehicleCardsContainer.innerHTML = '';
            
            vehiclesToShow.forEach(vehicle => {
                const featuresHTML = vehicle.features.map(feature => `
                    <li><i class="fas fa-check"></i> ${feature}</li>
                `).join('');
                
                const vehicleCard = document.createElement('div');
                vehicleCard.className = 'vehicle-card';
                vehicleCard.setAttribute('data-category', vehicle.category);
                
                vehicleCard.innerHTML = `
                    <div class="vehicle-icon">
                        <i class="fas fa-${vehicle.type === 'bus' ? 'bus' : 'car'}"></i>
                    </div>
                    <h3>${vehicle.name}</h3>
                    <p style="color: var(--gray-color); font-size: 0.9rem;">${vehicle.capacity}</p>
                    <div class="vehicle-price">$${vehicle.price}/day</div>
                    <p style="margin: 10px 0; font-size: 0.9rem;">${vehicle.description}</p>
                    <ul class="vehicle-features">
                        ${featuresHTML}
                    </ul>
                    <div class="vehicle-actions">
                        <button class="btn btn-secondary view-vehicle-btn" data-vehicle-id="${vehicle.id}">
                            <i class="fas fa-info-circle"></i> Details
                        </button>
                        <button class="btn book-vehicle-btn" data-vehicle-id="${vehicle.id}">
                            <i class="fas fa-car"></i> Book
                        </button>
                    </div>
                `;
                
                vehicleCardsContainer.appendChild(vehicleCard);
            });
            
            // Add event listeners to vehicle buttons
            document.querySelectorAll('.view-vehicle-btn').forEach(button => {
                button.addEventListener('click', function() {
                    const vehicleId = this.getAttribute('data-vehicle-id');
                    const vehicle = vehicles.find(v => v.id == vehicleId);
                    showVehicleDetailsModal(vehicle);
                });
            });
            
            document.querySelectorAll('.book-vehicle-btn').forEach(button => {
                button.addEventListener('click', function() {
                    const vehicleId = this.getAttribute('data-vehicle-id');
                    const vehicle = vehicles.find(v => v.id == vehicleId);
                    showVehicleBookingModal(vehicle);
                });
            });
        }

        // Generate rating stars HTML
        function generateRatingStars(rating) {
            let starsHTML = '';
            const fullStars = Math.floor(rating);
            const hasHalfStar = rating % 1 >= 0.5;
            
            for (let i = 0; i < 5; i++) {
                if (i < fullStars) {
                    starsHTML += '<i class="fas fa-star"></i>';
                } else if (i === fullStars && hasHalfStar) {
                    starsHTML += '<i class="fas fa-star-half-alt"></i>';
                } else {
                    starsHTML += '<i class="far fa-star"></i>';
                }
            }
            
            return starsHTML;
        }

        // Show vehicle details modal
        function showVehicleDetailsModal(vehicle) {
            const modalContent = document.getElementById('vehicleModalContent');
            const featuresHTML = vehicle.features.map(feature => `<li><i class="fas fa-check"></i> ${feature}</li>`).join('');
            
            modalContent.innerHTML = `
                <div style="text-align: center; margin-bottom: 20px;">
                    <div style="font-size: 3rem; color: var(--primary-color); margin-bottom: 10px;">
                        <i class="fas fa-${vehicle.type === 'bus' ? 'bus' : 'car'}"></i>
                    </div>
                    <h3>${vehicle.name}</h3>
                    <div class="vehicle-price">$${vehicle.price}/day</div>
                    <p>${vehicle.capacity}</p>
                </div>
                
                <div style="margin-bottom: 20px;">
                    <h4>Description</h4>
                    <p>${vehicle.description}</p>
                </div>
                
                <div style="margin-bottom: 20px;">
                    <h4>Features</h4>
                    <ul>
                        ${featuresHTML}
                    </ul>
                </div>
                
                <div style="background-color: #f9f9f9; padding: 15px; border-radius: var(--border-radius);">
                    <h4><i class="fas fa-info-circle"></i> Booking Information</h4>
                    <p>All our vehicles come with experienced Bhutanese drivers who know the roads and can share local insights. Fuel and driver accommodation are included in the price.</p>
                </div>
                
                <button class="btn" id="bookThisVehicle" data-vehicle-id="${vehicle.id}" style="width: 100%; margin-top: 20px;">
                    <i class="fas fa-car"></i> Book This Vehicle
                </button>
            `;
            
            // Add event listener to book button in modal
            document.getElementById('bookThisVehicle').addEventListener('click', function() {
                const vehicleId = this.getAttribute('data-vehicle-id');
                const vehicle = vehicles.find(v => v.id == vehicleId);
                vehicleModal.style.display = 'none';
                showVehicleBookingModal(vehicle);
            });
            
            vehicleModal.style.display = 'flex';
        }

        // Show vehicle booking modal
        function showVehicleBookingModal(vehicle) {
            const modalContent = document.getElementById('vehicleModalContent');
            
            modalContent.innerHTML = `
                <h4><i class="fas fa-car"></i> Book ${vehicle.name}</h4>
                <p><strong>Price:</strong> $${vehicle.price} per day</p>
                <p><strong>Capacity:</strong> ${vehicle.capacity}</p>
                
                <form id="vehicleBookingForm" style="margin-top: 20px;">
                    <div class="form-row">
                        <div class="form-group">
                            <label for="rentalDays">Rental Days</label>
                            <input type="number" id="rentalDays" class="form-control" min="1" max="30" value="7" required>
                        </div>
                        <div class="form-group">
                            <label for="rentalDate">Start Date</label>
                            <input type="date" id="rentalDate" class="form-control" required>
                        </div>
                    </div>
                    
                    <div class="form-group">
                        <label for="pickupLocation">Pickup Location</label>
                        <select id="pickupLocation" class="form-control" required>
                            <option value="">Select location</option>
                            <option value="paro_airport">Paro International Airport</option>
                            <option value="thimphu_hotel">Thimphu Hotel</option>
                            <option value="phuentsholing">Phuentsholing Border</option>
                            <option value="other">Other Location</option>
                        </select>
                    </div>
                    
                    <div class="form-group">
                        <label for="driverLanguage">Driver Language Preference</label>
                        <select id="driverLanguage" class="form-control">
                            <option value="english">English</option>
                            <option value="hindi">Hindi</option>
                            <option value="any">Any Language</option>
                        </select>
                    </div>
                    
                    <div class="form-note" style="margin-top: 15px;">
                        <i class="fas fa-info-circle"></i> Driver accommodation and meals are included. Fuel costs are covered for the itinerary.
                    </div>
                    
                    <button type="submit" class="btn" style="width: 100%; margin-top: 20px;">
                        <i class="fas fa-check"></i> Confirm Vehicle Booking
                    </button>
                </form>
            `;
            
            // Set min date for rental date
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('rentalDate').min = today;
            
            // Handle vehicle booking form submission
            document.getElementById('vehicleBookingForm').addEventListener('submit', function(e) {
                e.preventDefault();
                const days = parseInt(document.getElementById('rentalDays').value);
                const date = document.getElementById('rentalDate').value;
                const pickupLocation = document.getElementById('pickupLocation').value;
                const total = vehicle.price * days;
                
                // Store booking in localStorage
                localStorage.setItem('vehicleBooking', JSON.stringify({
                    vehicle: vehicle.name,
                    days: days,
                    date: date,
                    pickupLocation: pickupLocation,
                    total: total,
                    timestamp: new Date().toISOString()
                }));
                
                alert(`Vehicle booking confirmed!\n\n${vehicle.name} for ${days} day(s) starting ${date}\nPickup: ${pickupLocation}\nTotal: $${total}\n\nOur transport coordinator will contact you with driver details.`);
                vehicleModal.style.display = 'none';
                
                // Suggest adding to journey plan
                if (confirm('Would you like to add this vehicle to your Bhutan journey plan?')) {
                    document.getElementById('vehicleType').value = vehicle.type;
                    window.scrollTo({ top: document.getElementById('plan').offsetTop - 80, behavior: 'smooth' });
                }
            });
            
            vehicleModal.style.display = 'flex';
        }

        // Setup chat bot
        function setupChatBot() {
            // Toggle chat window
            chatbotToggle.addEventListener('click', function() {
                chatbotWindow.style.display = chatbotWindow.style.display === 'flex' ? 'none' : 'flex';
                if (chatbotWindow.style.display === 'flex') {
                    chatInput.focus();
                }
            });
            
            // Close chat window
            chatbotClose.addEventListener('click', function() {
                chatbotWindow.style.display = 'none';
            });
            
            // Send message on button click
            sendChat.addEventListener('click', sendChatMessage);
            
            // Send message on Enter key
            chatInput.addEventListener('keypress', function(e) {
                if (e.key === 'Enter') {
                    sendChatMessage();
                }
            });
            
            // Quick reply buttons
            document.querySelectorAll('.quick-reply').forEach(button => {
                button.addEventListener('click', function() {
                    const replyText = this.getAttribute('data-reply');
                    chatInput.value = replyText;
                    sendChatMessage();
                });
            });
        }

        // Send chat message
        function sendChatMessage() {
            const message = chatInput.value.trim();
            if (!message) return;
            
            // Add user message
            addMessageToChat(message, 'user');
            
            // Clear input
            chatInput.value = '';
            
            // Generate bot response after delay
            setTimeout(() => {
                generateBotResponse(message);
            }, 800);
        }

        // Add message to chat
        function addMessageToChat(text, sender) {
            const messageElement = document.createElement('div');
            messageElement.className = `message ${sender}-message`;
            messageElement.textContent = text;
            
            chatbotMessages.appendChild(messageElement);
            
            // Scroll to bottom
            chatbotMessages.scrollTop = chatbotMessages.scrollHeight;
        }

        // Generate bot response
        function generateBotResponse(userMessage) {
            const lowerMessage = userMessage.toLowerCase();
            let responseKey = "default";
            
            // Check for keywords
            const keywords = {
                "visa": "bhutan visa",
                "package": "tour packages",
                "tour": "tour packages",
                "time": "best time to visit",
                "season": "best time to visit",
                "festival": "festival dates",
                "cost": "cost",
                "price": "cost",
                "transport": "transport",
                "vehicle": "transport",
                "car": "transport",
                "trek": "trekking",
                "hike": "trekking",
                "culture": "culture",
                "hotel": "accommodation",
                "accommodation": "accommodation",
                "stay": "accommodation",
                "plan": "plan",
                "itinerary": "plan",
                "contact": "contact",
                "email": "contact",
                "phone": "contact"
            };
            
            for (const [keyword, response] of Object.entries(keywords)) {
                if (lowerMessage.includes(keyword)) {
                    responseKey = response;
                    break;
                }
            }
            
            // Special case for greetings
            if (lowerMessage.includes('hello') || lowerMessage.includes('hi') || lowerMessage.includes('hey') || lowerMessage.includes('tashi')) {
                responseKey = "greeting";
            }
            
            const responses = chatBotResponses[responseKey];
            const response = responses[Math.floor(Math.random() * responses.length)];
            
            // Add bot message
            addMessageToChat(response, 'bot');
            
            // Add quick replies for certain responses
            if (responseKey === "greeting" || responseKey === "default") {
                setTimeout(() => {
                    const quickRepliesHTML = `
                        <div class="quick-replies">
                            <div class="quick-reply" data-reply="Bhutan visa">Bhutan visa</div>
                            <div class="quick-reply" data-reply="Tour packages">Tour packages</div>
                            <div class="quick-reply" data-reply="Best time to visit">Best time</div>
                            <div class="quick-reply" data-reply="Festival dates">Festivals</div>
                        </div>
                    `;
                    
                    const quickRepliesContainer = document.createElement('div');
                    quickRepliesContainer.className = 'message bot-message';
                    quickRepliesContainer.innerHTML = quickRepliesHTML;
                    
                    chatbotMessages.appendChild(quickRepliesContainer);
                    
                    // Add event listeners to new quick reply buttons
                    quickRepliesContainer.querySelectorAll('.quick-reply').forEach(button => {
                        button.addEventListener('click', function() {
                            const replyText = this.getAttribute('data-reply');
                            chatInput.value = replyText;
                            sendChatMessage();
                        });
                    });
                    
                    // Scroll to bottom
                    chatbotMessages.scrollTop = chatbotMessages.scrollHeight;
                }, 300);
            }
        }

        // Set active nav item based on scroll position
        function setActiveNavItem() {
            let scrollPosition = window.scrollY + 100;
            
            // Get all sections
            const sections = document.querySelectorAll('section');
            
            sections.forEach(section => {
                const sectionTop = section.offsetTop;
                const sectionHeight = section.clientHeight;
                const sectionId = section.getAttribute('id');
                
                if (scrollPosition >= sectionTop && scrollPosition < sectionTop + sectionHeight) {
                    // Remove active class from all nav items
                    navItems.forEach(item => {
                        item.classList.remove('active');
                    });
                    
                    // Add active class to corresponding nav item
                    const activeNavItem = document.querySelector(`.nav-links a[href="#${sectionId}"]`);
                    if (activeNavItem) {
                        activeNavItem.classList.add('active');
                    }
                }
            });
        }
    </script>
</body>
</html>
