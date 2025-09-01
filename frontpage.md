<!DOCTYPE html>
<html lang="zh-Hant">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>首頁導覽列範例</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Inter', sans-serif;
            margin: 0;
            padding: 0;
        }
    </style>
</head>
<body>
    <!-- 導覽列 -->
    <header class="fixed top-0 left-0 w-full bg-black h-20 z-50">
        <div class="max-w-[1440px] mx-auto h-full flex items-center justify-between px-10">
            <!-- LOGO 變成首頁連結 -->
            <a href="/" class="flex-shrink-0">
                <img src="https://i.postimg.cc/QCKTgBMn/20240102-logo.png"
                     alt="LOGO"
                     class="w-[319px] h-[40px] object-contain">
            </a>
            <!-- 選單 -->
            <nav>
                <ul class="flex space-x-[34px] text-white font-bold text-[18px]">
                    <li><a href="#">課程總攬</a></li>
                    <li><a href="#">最新消息</a></li>
                    <li><a href="#">活動報名</a></li>
                    <li><a href="#">協會介紹</a></li>
                    <li><a href="#">聯絡我們</a></li>
                </ul>
            </nav>
        </div>
    </header>
</body>
</html>
<!-- Banner 區塊 -->
<section class="w-screen bg-[#012071] flex justify-center items-center" style="height:600px;">
    <!-- 搜尋框 -->
    <div class="flex items-center w-[90%] max-w-[400px] h-[50px] bg-white/20 rounded-[60px] px-4">
        <!-- 放大鏡 Icon -->
        <svg class="w-5 h-5 text-[#AFAFAF]" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M21 21l-4.35-4.35m0 0A7.5 7.5 0 1110.5 3a7.5 7.5 0 016.15 13.65z"/>
        </svg>
        <!-- 搜尋文字 -->
        <input type="text" placeholder="Search"
               class="ml-2 w-full bg-transparent border-none text-[#AFAFAF] placeholder-[#AFAFAF] text-[18px] font-normal focus:outline-none"/>
    </div>
</section>
<!-- 近期課程區塊 -->
<section class="mt-[56px] relative">
    <!-- 標題框 -->
    <div class="ml-[68px] w-[182px] h-[60px] bg-[#2759A7] rounded-[100px] flex items-center justify-center">
        <span class="font-bold text-[24px] text-white">近期課程</span>
    </div>

    <!-- 課程字卡區 -->
    <div class="flex mt-[65px] relative" style="margin-left:68px; gap:61px;">
        <!-- 課程1 -->
        <div class="w-[275px] h-[337px] bg-white rounded-[16px] shadow-[0_13px_25.2px_rgba(0,0,0,0.25)] transform-gpu transition-transform duration-300 hover:scale-[1.2]">
            <div class="w-[253px] h-[168px] rounded-[8px] bg-gray-200 mx-[13px] mt-[15px]"></div>
            <h3 class="mt-4 mx-[13px] text-[16px] font-bold text-black">課程1</h3>
            <p class="mt-2 mx-[13px] text-[12px] font-medium text-black">文文文文文文文文文文文</p>
        </div>

        <!-- 課程2 -->
        <div class="w-[275px] h-[337px] bg-white rounded-[16px] shadow-[0_13px_25.2px_rgba(0,0,0,0.25)] transform-gpu transition-transform duration-300 hover:scale-[1.2]">
            <div class="w-[253px] h-[168px] rounded-[8px] bg-gray-200 mx-[13px] mt-[15px]"></div>
            <h3 class="mt-4 mx-[13px] text-[16px] font-bold text-black">課程2</h3>
            <p class="mt-2 mx-[13px] text-[12px] font-medium text-black">文文文文文文文文文文文</p>
        </div>

        <!-- 課程3 -->
        <div class="w-[275px] h-[337px] bg-white rounded-[16px] shadow-[0_13px_25.2px_rgba(0,0,0,0.25)] transform-gpu transition-transform duration-300 hover:scale-[1.2]">
            <div class="w-[253px] h-[168px] rounded-[8px] bg-gray-200 mx-[13px] mt-[15px]"></div>
            <h3 class="mt-4 mx-[13px] text-[16px] font-bold text-black">課程3</h3>
            <p class="mt-2 mx-[13px] text-[12px] font-medium text-black">文文文文文文文文文文文</p>
        </div>

        <!-- 課程4 -->
        <div id="course4" class="w-[275px] h-[337px] bg-white rounded-[16px] shadow-[0_13px_25.2px_rgba(0,0,0,0.25)] transform-gpu transition-transform duration-300 hover:scale-[1.2] relative">
            <div class="w-[253px] h-[168px] rounded-[8px] bg-gray-200 mx-[13px] mt-[15px]"></div>
            <h3 class="mt-4 mx-[13px] text-[16px] font-bold text-black">課程4</h3>
            <p class="mt-2 mx-[13px] text-[12px] font-medium text-black">文文文文文文文文文文文</p>
        </div>
    </div>

    <!-- 瀏覽更多按鈕，固定在課程4右下方，不受字卡放大影響 -->
    <a href="#"
       class="absolute w-[108px] h-[48px] flex items-center justify-center border-2 border-[#2759A7] rounded-[100px] text-[#2759A7] font-semibold text-[13px]"
       style="top: 525px; left: calc(68px + 814px + 361px);">
        瀏覽更多
    </a>
</section>

   <!-- 新聞消息區塊 -->
<section class="mt-[154px] relative">
    <!-- 標題框 -->
    <div class="ml-[68px] w-[182px] h-[60px] bg-[#2759A7] rounded-[100px] flex items-center justify-center">
        <span class="font-bold text-[24px] text-white">新聞消息</span>
    </div>

    <!-- 消息卡片區 -->
    <div class="flex mt-[65px] relative" style="margin-left:68px; gap:36px;">
        <!-- 消息1 -->
        <div class="w-[290px] h-[283px] rounded-[16px] relative overflow-hidden group cursor-pointer">
            <div class="w-[261px] h-[164.73px] bg-gray-200 rounded-[8px] mx-auto mt-[15px]"></div>
            <h3 class="mt-[23px] text-[16px] font-bold text-black text-left ml-[14.5px]">消息1</h3>
            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-20 flex items-start justify-start pt-4 px-4 text-white text-left opacity-0 group-hover:opacity-100 transition-opacity">
                簡單說明
            </div>
        </div>

        <!-- 消息2 -->
        <div class="w-[290px] h-[283px] rounded-[16px] relative overflow-hidden group cursor-pointer">
            <div class="w-[261px] h-[164.73px] bg-gray-200 rounded-[8px] mx-auto mt-[15px]"></div>
            <h3 class="mt-[23px] text-[16px] font-bold text-black text-left ml-[14.5px]">消息2</h3>
            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-20 flex items-start justify-start pt-4 px-4 text-white text-left opacity-0 group-hover:opacity-100 transition-opacity">
                簡單說明
            </div>
        </div>

        <!-- 消息3 -->
        <div class="w-[290px] h-[283px] rounded-[16px] relative overflow-hidden group cursor-pointer">
            <div class="w-[261px] h-[164.73px] bg-gray-200 rounded-[8px] mx-auto mt-[15px]"></div>
            <h3 class="mt-[23px] text-[16px] font-bold text-black text-left ml-[14.5px]">消息3</h3>
            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-20 flex items-start justify-start pt-4 px-4 text-white text-left opacity-0 group-hover:opacity-100 transition-opacity">
                簡單說明
            </div>
        </div>

        <!-- 消息4 -->
        <div id="message4" class="w-[290px] h-[283px] rounded-[16px] relative overflow-hidden group cursor-pointer">
            <div class="w-[261px] h-[164.73px] bg-gray-200 rounded-[8px] mx-auto mt-[15px]"></div>
            <h3 class="mt-[23px] text-[16px] font-bold text-black text-left ml-[14.5px]">消息4</h3>
            <div class="absolute inset-0 bg-black bg-opacity-0 group-hover:bg-opacity-20 flex items-start justify-start pt-4 px-4 text-white text-left opacity-0 group-hover:opacity-100 transition-opacity">
                簡單說明
            </div>
        </div>

        <!-- 瀏覽更多按鈕，獨立於消息4，不受 hover 影響 -->
        <a href="#"
           class="absolute w-[108px] h-[48px] flex items-center justify-center border-2 border-[#2759A7] rounded-[100px] text-[#2759A7] font-semibold text-[13px]"
           style="bottom:-58px; right:0;">
            瀏覽更多
        </a>
    </div>
</section>

<!-- 頁尾區塊 -->
<footer class="w-full h-[320px] bg-white shadow-[0_-5px_10px_rgba(0,0,0,0.25)] flex items-center">
    <div class="ml-[190px] text-[14px] font-medium text-[#6C6C6D]">
        <div class="flex items-center gap-[8px] mb-[12px]">
            <span class="w-[60px] inline-block">MAIL</span>
            <span class="inline-block">服務信箱</span>
            <span class="mx-[8px]">｜</span>
        </div>
        <div class="flex items-center gap-[8px] mb-[12px]">
            <span class="w-[60px] inline-block">PHONE</span>
            <span class="inline-block">客服專線</span>
            <span class="mx-[8px]">｜</span>
            <span class="inline-block">02-XXXXXXX</span>
        </div>
        <div class="flex items-center gap-[8px] mb-[12px]">
            <span class="w-[60px] inline-block">TIME</span>
            <span class="inline-block">客服時間</span>
            <span class="mx-[8px]">｜</span>
        </div>
        <div class="flex items-center gap-[8px]">
            <span class="w-[60px] inline-block">ADDRESS</span>
            <span class="inline-block">服務地址</span>
        </div>
    </div>
</footer>
