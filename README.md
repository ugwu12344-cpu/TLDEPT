<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>"Bag Chaser" Sturdy Case - TLDept</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Inter', sans-serif; }
        
        /* Marquee Animation */
        @keyframes marquee {
            0% { transform: translateX(0); }
            100% { transform: translateX(-50%); }
        }
        .marquee-track {
            animation: marquee 20s linear infinite;
        }
        
        /* Smooth Accordion */
        .accordion-content {
            max-height: 0;
            overflow: hidden;
            transition: max-height 0.3s ease-out, padding 0.3s ease;
        }
        .accordion-content.active {
            max-height: 500px;
        }
        
        /* Image Gallery Fade */
        .gallery-fade {
            opacity: 0;
            transition: opacity 0.3s ease;
        }
        .gallery-fade.active {
            opacity: 1;
        }
        
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: #888;
            border-radius: 4px;
        }
        
        /* Hover Effects */
        .product-card {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .product-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 40px rgba(0,0,0,0.1);
        }
        
        /* Button Ripple */
        .btn-primary {
            position: relative;
            overflow: hidden;
        }
        .btn-primary::after {
            content: '';
            position: absolute;
            top: 50%;
            left: 50%;
            width: 0;
            height: 0;
            border-radius: 50%;
            background: rgba(255,255,255,0.3);
            transform: translate(-50%, -50%);
            transition: width 0.6s, height 0.6s;
        }
        .btn-primary:active::after {
            width: 300px;
            height: 300px;
        }
    </style>
</head>
<body class="bg-white text-black">

    <!-- Announcement Bar -->
    <div class="bg-black text-white overflow-hidden py-2 relative">
        <div class="marquee-track flex whitespace-nowrap">
            <span class="mx-8 text-xs font-bold tracking-wider flex items-center gap-2">
                🔥 HUGE 35% OFF ALL CASES! 🔥
            </span>
            <span class="mx-8 text-xs font-bold tracking-wider flex items-center gap-2">
                🚚 FREE SHIPPING ON ORDERS OVER $50 🚚
            </span>
            <span class="mx-8 text-xs font-bold tracking-wider flex items-center gap-2">
                🔥 HUGE 35% OFF ALL CASES! 🔥
            </span>
            <span class="mx-8 text-xs font-bold tracking-wider flex items-center gap-2">
                🚚 FREE SHIPPING ON ORDERS OVER $50 🚚
            </span>
            <span class="mx-8 text-xs font-bold tracking-wider flex items-center gap-2">
                🔥 HUGE 35% OFF ALL CASES! 🔥
            </span>
            <span class="mx-8 text-xs font-bold tracking-wider flex items-center gap-2">
                🚚 FREE SHIPPING ON ORDERS OVER $50 🚚
            </span>
            <span class="mx-8 text-xs font-bold tracking-wider flex items-center gap-2">
                🔥 HUGE 35% OFF ALL CASES! 🔥
            </span>
            <span class="mx-8 text-xs font-bold tracking-wider flex items-center gap-2">
                🚚 FREE SHIPPING ON ORDERS OVER $50 🚚
            </span>
        </div>
    </div>

    <!-- Navigation -->
    <nav class="sticky top-0 z-50 bg-white/95 backdrop-blur-md border-b border-gray-100">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-16">
                <!-- Mobile Menu -->
                <button class="p-2 hover:bg-gray-100 rounded-lg transition-colors">
                    <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"/>
                    </svg>
                </button>
                
                <!-- Logo -->
                <div class="flex-1 flex justify-center">
                    <h1 class="text-2xl font-black tracking-tighter italic">TLDEPT</h1>
                </div>
                
                <!-- Right Icons -->
                <div class="flex items-center gap-4">
                    <button class="text-sm font-medium hover:text-gray-600 transition-colors hidden sm:block">
                        USD $ | United States ▼
                    </button>
                    <button class="p-2 hover:bg-gray-100 rounded-full transition-colors">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>
                        </svg>
                    </button>
                    <button class="p-2 hover:bg-gray-100 rounded-full transition-colors relative">
                        <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z"/>
                        </svg>
                        <span class="absolute -top-1 -right-1 bg-black text-white text-xs w-5 h-5 flex items-center justify-center rounded-full">0</span>
                    </button>
                </div>
            </div>
        </div>
    </nav>

    <!-- Main Product Section -->
    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8">
        <div class="lg:grid lg:grid-cols-2 lg:gap-12">
            
            <!-- Left: Image Gallery -->
            <div class="space-y-4">
                <!-- Main Image -->
                <div class="relative aspect-square bg-gray-50 rounded-2xl overflow-hidden group">
                    <img id="mainImage" 
                         src="https://images.unsplash.com/photo-1603313011101-320f26a4f6f6?w=800&auto=format&fit=crop&q=80" 
                         alt="Bag Chaser Case" 
                         class="w-full h-full object-contain p-8 gallery-fade active transition-transform duration-500 group-hover:scale-105">
                    
                    <!-- Image Navigation Arrows -->
                    <button onclick="changeImage(-1)" class="absolute left-4 top-1/2 -translate-y-1/2 bg-white/80 hover:bg-white p-2 rounded-full shadow-lg opacity-0 group-hover:opacity-100 transition-opacity">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"/></svg>
                    </button>
                    <button onclick="changeImage(1)" class="absolute right-4 top-1/2 -translate-y-1/2 bg-white/80 hover:bg-white p-2 rounded-full shadow-lg opacity-0 group-hover:opacity-100 transition-opacity">
                        <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/></svg>
                    </button>
                </div>
                
                <!-- Thumbnail Grid -->
                <div class="grid grid-cols-4 gap-3">
                    <button onclick="setImage(0)" class="aspect-square bg-gray-50 rounded-lg overflow-hidden border-2 border-black hover:opacity-80 transition-opacity">
                        <img src="https://images.unsplash.com/photo-1603313011101-320f26a4f6f6?w=200&auto=format&fit=crop&q=80" class="w-full h-full object-contain p-2">
                    </button>
                    <button onclick="setImage(1)" class="aspect-square bg-gray-50 rounded-lg overflow-hidden border-2 border-transparent hover:border-gray-300 transition-all">
                        <img src="https://images.unsplash.com/photo-1586105251261-72a756497a11?w=200&auto=format&fit=crop&q=80" class="w-full h-full object-contain p-2">
                    </button>
                    <button onclick="setImage(2)" class="aspect-square bg-gray-50 rounded-lg overflow-hidden border-2 border-transparent hover:border-gray-300 transition-all">
                        <img src="https://images.unsplash.com/photo-1592899677977-9c10ca588bbd?w=200&auto=format&fit=crop&q=80" class="w-full h-full object-contain p-2">
                    </button>
                    <button onclick="setImage(3)" class="aspect-square bg-gray-50 rounded-lg overflow-hidden border-2 border-transparent hover:border-gray-300 transition-all">
                        <img src="https://images.unsplash.com/photo-1511707171634-5f897ff02aa9?w=200&auto=format&fit=crop&q=80" class="w-full h-full object-contain p-2">
                    </button>
                </div>
            </div>

            <!-- Right: Product Details -->
            <div class="mt-8 lg:mt-0 space-y-6">
                <div>
                    <h1 class="text-3xl sm:text-4xl font-bold leading-tight">"Bag Chaser"<br>Sturdy Case</h1>
                    <div class="mt-4 flex items-baseline gap-3">
                        <span
