# Liora-reservation
<!DOCTYPE html>
<html lang="zh-TW">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>我的 Netlify 專案 - 簡介</title>
    <!-- 載入 Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- 設定 Tailwind 配置，使用 Inter 字體 -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Inter', 'Noto Sans TC', 'sans-serif'],
                    },
                    colors: {
                        'primary': '#4F46E5', // Indigo-600
                        'secondary': '#10B981', // Emerald-500
                    }
                }
            }
        }
    </script>
    <style>
        /* 自定義樣式: 確保頁面最小高度 */
        body {
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            background-color: #F9FAFB; /* Light Gray Background */
        }
        /* 簡單的按鈕懸停效果 */
        .btn-primary {
            transition: transform 0.2s, box-shadow 0.2s;
        }
        .btn-primary:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -2px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body class="font-sans antialiased">

    <!-- 主要內容區塊 -->
    <main class="flex-grow flex items-center justify-center p-4 sm:p-6 lg:p-8">
        <div class="w-full max-w-4xl bg-white shadow-xl rounded-2xl overflow-hidden md:flex">
            
            <!-- 左側個人資訊/圖片區塊 (在手機上會堆疊在上方) -->
            <div class="md:w-1/3 bg-primary p-8 flex flex-col items-center justify-center text-white text-center">
                <!-- 頭像 Placeholder -->
                <div class="w-32 h-32 bg-indigo-300 rounded-full flex items-center justify-center mb-4 border-4 border-white shadow-lg">
                    <svg class="w-16 h-16" fill="currentColor" viewBox="0 0 24 24">
                        <path d="M12 12c2.21 0 4-1.79 4-4s-1.79-4-4-4-4 1.79-4 4 1.79 4 4 4zm0 2c-2.67 0-8 1.34-8 4v2h16v-2c0-2.66-5.33-4-8-4z"/>
                    </svg>
                </div>
                <h1 class="text-2xl font-bold">陳莉娜 (LiNa Chen)</h1>
                <p class="text-indigo-200 mt-1">前端開發者 / UX/UI 愛好者</p>
                
                <div class="mt-6">
                    <a href="#" class="inline-block mx-2 text-indigo-100 hover:text-white transition duration-150">
                        <!-- 範例圖示：GitHub (使用 Lucide icon 樣式) -->
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M15 22v-4a4.8 4.8 0 0 0-1-3.5c3 0 6-2 6-5.5.08-1.25-.27-2.44-1-3.5.25-1.02.24-2.19-.11-3.32 0 0-1 0-3 1.5-2.64-.5-5.36-.5-8 0C6 2 5 2 5 2c-.36 1.13-.37 2.3-.11 3.32-.73 1.06-1.18 2.25-1 3.5 0 3.5 3 5.5 6 5.5-.39.49-.68 1.05-.85 1.65-.17.6-.22 1.25-.22 1.9V22"/></svg>
                    </a>
                    <a href="#" class="inline-block mx-2 text-indigo-100 hover:text-white transition duration-150">
                        <!-- 範例圖示：LinkedIn -->
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect width="4" height="12" x="2" y="9"/><circle cx="4" cy="4" r="2"/></svg>
                    </a>
                </div>
            </div>

            <!-- 右側詳細內容區塊 -->
            <div class="md:w-2/3 p-8">
                <h2 class="text-3xl font-extrabold text-gray-800 mb-6">關於我</h2>
                
                <p class="text-gray-600 mb-6 leading-relaxed">
                    我是一位熱衷於打造優雅、高效能且用戶友好的網頁體驗的開發者。
                    專注於現代 JavaScript 框架（例如 React/Vue）的應用，並對網站效能優化和響應式設計有深入的理解。
                    期待利用技術來解決實際問題，並持續學習新的技術趨勢。
                </p>

                <!-- 技能區塊 -->
                <div class="mb-8">
                    <h3 class="text-xl font-semibold text-gray-700 mb-3 border-b pb-1">核心技能</h3>
                    <div class="flex flex-wrap gap-2">
                        <span class="px-3 py-1 bg-secondary text-white text-sm font-medium rounded-full shadow-md">HTML5 / CSS3</span>
                        <span class="px-3 py-1 bg-secondary text-white text-sm font-medium rounded-full shadow-md">JavaScript (ES6+)</span>
                        <span class="px-3 py-1 bg-secondary text-white text-sm font-medium rounded-full shadow-md">React.js</span>
                        <span class="px-3 py-1 bg-secondary text-white text-sm font-medium rounded-full shadow-md">Tailwind CSS</span>
                        <span class="px-3 py-1 bg-secondary text-white text-sm font-medium rounded-full shadow-md">Git / Netlify</span>
                    </div>
                </div>

                <!-- 聯絡按鈕 -->
                <div class="mt-6 pt-4 border-t">
                    <h3 class="text-xl font-semibold text-gray-700 mb-3">聯繫我</h3>
                    <a href="mailto:your.email@example.com" class="btn-primary inline-flex items-center bg-primary text-white font-bold py-3 px-6 rounded-xl shadow-lg hover:bg-indigo-700 focus:outline-none focus:ring-4 focus:ring-indigo-500 focus:ring-opacity-50">
                        <svg xmlns="http://www.w3.org/2000/svg" class="h-5 w-5 mr-2" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2"><path stroke-linecap="round" stroke-linejoin="round" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8m-1 12H4a2 2 0 01-2-2V6a2 2 0 012-2h16a2 2 0 012 2v12a2 2 0 01-2 2z"/></svg>
                        發送郵件
                    </a>
                </div>
            </div>
            
        </div>
    </main>

    <!-- 頁腳 -->
    <footer class="text-center p-4 text-gray-500 text-sm">
        <p>&copy; <span id="currentYear"></span> 陳莉娜. 保留所有權利。</p>
    </footer>

    <!-- JavaScript 腳本 -->
    <script>
        // 設置當前年份
        document.getElementById('currentYear').textContent = new Date().getFullYear();

        // 這裡可以添加更多的交互式 JavaScript
        function showMessage(title, message) {
            console.log(`${title}: ${message}`);
        }
    </script>
</body>
</html>

