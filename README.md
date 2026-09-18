<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Smart Adaptive Assessment & Learning Analytics Platform</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Prompt Font -->
    <link href="https://fonts.googleapis.com/css2?family=Prompt:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Prompt', sans-serif; }
    </style>
</head>
<body class="bg-slate-50 text-slate-800 min-h-screen">

    <!-- Header / Navbar -->
    <header class="bg-indigo-700 text-white shadow-lg sticky top-0 z-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-3">
                <i class="fa-solid fa-brain text-yellow-300 text-2xl"></i>
                <h1 class="text-xl font-bold tracking-wide">Smart Adaptive Assessment Platform</h1>
            </div>
            <span class="bg-indigo-800 text-indigo-100 text-xs px-3 py-1 rounded-full border border-indigo-500">
                Learning Analytics Platform
            </span>
        </div>
    </header>

    <main class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 space-y-10">

        <!-- SECTION 1: TEACHER DASHBOARD (ภาพรวมชั้นเรียน) -->
        <section>
            <div class="flex items-center justify-between mb-6">
                <div>
                    <h2 class="text-2xl font-bold text-slate-900 flex items-center gap-2">
                        <i class="fa-solid fa-chart-line text-indigo-600"></i> Teacher Dashboard (ภาพรวมห้องเรียน)
                    </h2>
                    <p class="text-sm text-slate-500">สรุปผลการประเมินและวิเคราะห์พัฒนาการผู้เรียนทั้งหมด</p>
                </div>
                <span class="text-sm font-medium bg-white px-4 py-2 rounded-lg border border-slate-200 shadow-sm">
                    นักเรียนทั้งหมด: <strong class="text-indigo-600 font-bold">38 คน</strong>
                </span>
            </div>

            <!-- Stats Overview Cards -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6 mb-8">
                <!-- Card Total -->
                <div class="bg-white rounded-xl p-6 shadow-sm border border-slate-200 flex items-center justify-between">
                    <div>
                        <p class="text-sm font-medium text-slate-500">นักเรียนทั้งหมด</p>
                        <p class="text-3xl font-extrabold text-slate-800 mt-1">38 <span class="text-base font-normal text-slate-500">คน</span></p>
                    </div>
                    <div class="w-12 h-12 bg-blue-50 text-blue-600 rounded-full flex items-center justify-center text-xl">
                        <i class="fa-solid fa-users"></i>
                    </div>
                </div>

                <!-- Card Passed -->
                <div class="bg-white rounded-xl p-6 shadow-sm border border-emerald-100 flex items-center justify-between">
                    <div>
                        <p class="text-sm font-medium text-emerald-600">ผ่านเกณฑ์</p>
                        <p class="text-3xl font-extrabold text-emerald-600 mt-1">30 <span class="text-base font-normal text-slate-500">คน (78.9%)</span></p>
                    </div>
                    <div class="w-12 h-12 bg-emerald-50 text-emerald-600 rounded-full flex items-center justify-center text-xl">
                        <i class="fa-solid fa-circle-check"></i>
                    </div>
                </div>

                <!-- Card Need Development -->
                <div class="bg-white rounded-xl p-6 shadow-sm border border-rose-100 flex items-center justify-between">
                    <div>
                        <p class="text-sm font-medium text-rose-600">ต้องพัฒนา</p>
                        <p class="text-3xl font-extrabold text-rose-600 mt-1">8 <span class="text-base font-normal text-slate-500">คน (21.1%)</span></p>
                    </div>
                    <div class="w-12 h-12 bg-rose-50 text-rose-600 rounded-full flex items-center justify-center text-xl">
                        <i class="fa-solid fa-triangle-exclamation"></i>
                    </div>
                </div>
            </div>

            <!-- Class Progress Bar -->
            <div class="bg-white p-6 rounded-xl shadow-sm border border-slate-200">
                <div class="flex justify-between items-center mb-2">
                    <span class="text-sm font-semibold text-slate-700">สัดส่วนผลการประเมินรวม</span>
                    <span class="text-xs text-slate-500">ผ่านเกณฑ์ 30 / ต้องพัฒนา 8</span>
                </div>
                <div class="w-full bg-rose-200 rounded-full h-4 overflow-hidden flex">
                    <div class="bg-emerald-500 h-4 transition-all duration-500" style="width: 78.95%" title="ผ่านเกณฑ์ 30 คน"></div>
                    <div class="bg-rose-500 h-4 transition-all duration-500" style="width: 21.05%" title="ต้องพัฒนา 8 คน"></div>
                </div>
                <div class="flex gap-6 mt-3 text-xs text-slate-600">
                    <span class="flex items-center gap-1.5"><i class="fa-solid fa-square text-emerald-500"></i> ผ่านเกณฑ์ (30 คน)</span>
                    <span class="flex items-center gap-1.5"><i class="fa-solid fa-square text-rose-500"></i> ต้องพัฒนา (8 คน)</span>
                </div>
            </div>
        </section>

        <hr class="border-slate-200">

        <!-- SECTION 2: STUDENT DASHBOARD (มุมมองนักเรียนรายบุคคล) -->
        <section>
            <div class="flex items-center justify-between mb-6">
                <div>
                    <h2 class="text-2xl font-bold text-slate-900 flex items-center gap-2">
                        <i class="fa-solid fa-user-graduate text-indigo-600"></i> Student Dashboard (มุมมองนักเรียน)
                    </h2>
                    <p class="text-sm text-slate-500">ข้อมูลการวิเคราะห์ผลการเรียนรู้เฉพาะบุคคล</p>
                </div>
            </div>

            <!-- Student Profile Header -->
            <div class="bg-indigo-900 text-white rounded-2xl p-6 shadow-md mb-6 relative overflow-hidden">
                <div class="absolute -right-10 -bottom-10 opacity-10 text-9xl">
                    <i class="fa-solid fa-graduation-cap"></i>
                </div>
                <div class="flex flex-col sm:flex-row items-start sm:items-center justify-between gap-4 relative z-10">
                    <div class="flex items-center space-x-4">
                        <div class="w-16 h-16 bg-indigo-500 border-2 border-indigo-300 rounded-full flex items-center justify-center text-2xl font-bold text-white shadow">
                            นต
                        </div>
                        <div>
                            <h3 class="text-xl font-bold">นางสาวนารีรัตน์ ตัญญาภักดิ์</h3>
                            <p class="text-indigo-200 text-sm">รหัสประจำตัว: STD-202638 | ชั้นมัธยมศึกษาปีที่ 6</p>
                        </div>
                    </div>
                    <div>
                        <span class="bg-emerald-500 text-white text-sm font-semibold px-4 py-2 rounded-full shadow-sm flex items-center gap-2">
                            <i class="fa-solid fa-circle-check"></i> สถานะ: ผ่านเกณฑ์
                        </span>
                    </div>
                </div>
            </div>

            <!-- Student Analytics Grid -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-6">
                <!-- Score & Progress -->
                <div class="bg-white p-5 rounded-xl border border-slate-200 shadow-sm">
                    <div class="flex items-center justify-between text-slate-500 mb-2">
                        <span class="text-sm font-medium">คะแนนรวมสะสม</span>
                        <i class="fa-solid fa-star text-amber-400"></i>
                    </div>
                    <p class="text-2xl font-bold text-slate-800">85 / 100</p>
                    <div class="mt-3">
                        <div class="flex justify-between text-xs text-slate-500 mb-1">
                            <span>ความก้าวหน้า</span>
                            <span>85%</span>
                        </div>
                        <div class="w-full bg-slate-100 rounded-full h-2">
                            <div class="bg-indigo-600 h-2 rounded-full" style="width: 85%"></div>
                        </div>
                    </div>
                </div>

                <!-- Learning Time -->
                <div class="bg-white p-5 rounded-xl border border-slate-200 shadow-sm">
                    <div class="flex items-center justify-between text-slate-500 mb-2">
                        <span class="text-sm font-medium">เวลาเรียนรวม</span>
                        <i class="fa-solid fa-clock text-blue-500"></i>
                    </div>
                    <p class="text-2xl font-bold text-slate-800">14 ชม. 45 นาที</p>
                    <p class="text-xs text-emerald-600 mt-2 flex items-center gap-1">
                        <i class="fa-solid fa-arrow-trend-up"></i> ต่อเนื่องตามเกณฑ์มาตรฐาน
                    </p>
                </div>

                <!-- Attempts & Accuracy -->
                <div class="bg-white p-5 rounded-xl border border-slate-200 shadow-sm">
                    <div class="flex items-center justify-between text-slate-500 mb-2">
                        <span class="text-sm font-medium">ความแม่นยำ (Accuracy)</span>
                        <i class="fa-solid fa-bullseye text-emerald-500"></i>
                    </div>
                    <p class="text-2xl font-bold text-slate-800">88.5%</p>
                    <p class="text-xs text-slate-500 mt-2">ทำแบบทดสอบซ้ำเฉลี่ย: <strong>1.2 ครั้ง/บท</strong></p>
                </div>

                <!-- Weakness Alert -->
                <div class="bg-white p-5 rounded-xl border border-slate-200 shadow-sm">
                    <div class="flex items-center justify-between text-slate-500 mb-2">
                        <span class="text-sm font-medium">จุดอ่อนที่ต้องทบทวน</span>
                        <i class="fa-solid fa-bug text-rose-500"></i>
                    </div>
                    <p class="text-lg font-bold text-rose-600 truncate">การประยุกต์ใช้พีชคณิต</p>
                    <p class="text-xs text-slate-500 mt-2">พบข้อผิดพลาดในแบบทดสอบล่าสุด</p>
                </div>
            </div>

            <!-- Weakness & Remedial Path Detail -->
            <div class="bg-white rounded-xl p-6 border border-slate-200 shadow-sm space-y-4">
                <h4 class="font-bold text-slate-800 text-lg flex items-center gap-2">
                    <i class="fa-solid fa-lightbulb text-yellow-500"></i> เส้นทางการเรียนรู้ที่แนะนำ (Adaptive Learning Path)
                </h4>
                <p class="text-sm text-slate-600">
                    ระบบวิเคราะห์ว่า <strong class="text-slate-800">นางสาวนารีรัตน์ ตัญญาภักดิ์</strong> มีความเข้าใจดีเยี่ยมในเนื้อหาทั่วไป แต่สามารถพัฒนาเพิ่มเติมในหัวข้อเฉพาะด้านได้ดังนี้:
                </p>

                <div class="grid grid-cols-1 md:grid-cols-2 gap-4 pt-2">
                    <!-- Recommended Module 1 -->
                    <div class="border border-slate-200 rounded-lg p-4 bg-slate-50 flex justify-between items-center">
                        <div>
                            <span class="bg-amber-100 text-amber-800 text-xs px-2.5 py-0.5 rounded font-medium">ควรทบทวนเพิ่ม</span>
                            <h5 class="font-semibold text-slate-800 mt-1">การแก้โจทย์ปัญหาพีชคณิตเชิงซ้อน</h5>
                            <p class="text-xs text-slate-500 mt-1">ใช้เวลาแนะนำ: 15 นาที</p>
                        </div>
                        <button class="bg-indigo-600 hover:bg-indigo-700 text-white text-xs px-3 py-2 rounded-lg transition">
                            เรียนทันที
                        </button>
                    </div>

                    <!-- Recommended Module 2 -->
                    <div class="border border-slate-200 rounded-lg p-4 bg-slate-50 flex justify-between items-center">
                        <div>
                            <span class="bg-emerald-100 text-emerald-800 text-xs px-2.5 py-0.5 rounded font-medium">แบบฝึกท้าทาย</span>
                            <h5 class="font-semibold text-slate-800 mt-1">โจทย์ประยุกต์ระดับสูง (Advanced)</h5>
                            <p class="text-xs text-slate-500 mt-1">ส่งเสริมศักยภาพกลุ่มผ่านเกณฑ์</p>
                        </div>
                        <button class="bg-slate-800 hover:bg-slate-900 text-white text-xs px-3 py-2 rounded-lg transition">
                            เริ่มทำโจทย์
                        </button>
                    </div>
                </div>
            </div>
        </section>

    </main>

    <!-- Footer -->
    <footer class="bg-white border-t border-slate-200 mt-12 py-6 text-center text-xs text-slate-500">
        <p>© 2026 Smart Adaptive Assessment & Learning Analytics Platform. All rights reserved.</p>
    </footer>

</body>
</html>
