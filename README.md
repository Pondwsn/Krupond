<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>เว็บไซต์สรุปกฎหมายข้าราชการที่ดี</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=IBM+Plex+Sans+Thai:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'IBM Plex Sans Thai', sans-serif;
            background-color: #f1f5f9;
        }
        /* Simple fade-in animation */
        .fade-in {
            animation: fadeIn 0.5s ease-in-out;
        }
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .card-hover {
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgb(0 0 0 / 0.1), 0 4px 6px -4px rgb(0 0 0 / 0.1);
        }
    </style>
</head>
<body>

    <div id="app" class="container mx-auto p-4 md:p-8">
        <!-- Content will be rendered here by JavaScript -->
    </div>

    <script>
        // --- DATA ---
        const laws = {
            'pobor': {
                title: 'พ.ร.บ. บริหารราชการแผ่นดิน',
                short_desc: 'วางโครงสร้างการบริหารประเทศ 3 ส่วน',
                icon: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#3b82f6" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polygon points="12 2 2 7 12 12 22 7 12 2"></polygon><polyline points="2 17 12 22 22 17"></polyline><polyline points="2 12 12 17 22 12"></polyline></svg>',
                color: 'blue',
                details: `
                    <h3 class="text-2xl font-bold text-blue-800 mb-4">พ.ร.บ. ระเบียบบริหารราชการแผ่นดิน พ.ศ. 2534</h3>
                    <p class="mb-4 text-gray-600">เป็นกฎหมายหลักที่วางโครงสร้างการบริหารประเทศ โดยมีนายกรัฐมนตรีเป็นผู้รักษาการ</p>
                    <div class="space-y-4">
                        <div>
                            <h4 class="font-semibold text-lg text-blue-700">🎯 หลักการสำคัญ</h4>
                            <ul class="list-disc list-inside mt-2 text-gray-600 space-y-1">
                                <li><b>เป้าหมายสูงสุด:</b> เพื่อประโยชน์สุขของประชาชน เกิดผลสัมฤทธิ์ต่อภารกิจรัฐ มีประสิทธิภาพ คุ้มค่า ลดขั้นตอน และอำนวยความสะดวก</li>
                                <li><b>การบริหารราชการแบ่งเป็น 3 ส่วน:</b>
                                    <ol class="list-decimal list-inside ml-4 mt-1">
                                        <li><b>ส่วนกลาง (หลักรวมอำนาจ):</b> อำนาจตัดสินใจอยู่ที่ส่วนกลาง ได้แก่ สำนักนายกรัฐมนตรี, กระทรวง, ทบวง, กรม (ทุกส่วนนี้มีฐานะเป็น <b>นิติบุคคล</b>)</li>
                                        <li><b>ส่วนภูมิภาค (หลักแบ่งอำนาจ):</b> แบ่งอำนาจจากส่วนกลางไปให้เจ้าหน้าที่ในพื้นที่ ได้แก่ <b>จังหวัด</b> (มีฐานะเป็นนิติบุคคล) และ <b>อำเภอ</b> (ไม่มีฐานะเป็นนิติบุคคล)</li>
                                        <li><b>ส่วนท้องถิ่น (หลักกระจายอำนาจ):</b> ให้ประชาชนในท้องถิ่นปกครองตนเองอย่างอิสระ ได้แก่ อบจ., เทศบาล, อบต. และรูปแบบพิเศษ (กทม., พัทยา)</li>
                                    </ol>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <h4 class="font-semibold text-lg text-blue-700">🔑 ประเด็นน่าจำ</h4>
                            <ul class="list-disc list-inside mt-2 text-gray-600 space-y-1">
                                <li><b>การตั้ง/ยุบ/เปลี่ยนเขตจังหวัด:</b> ต้องตราเป็น <b>พระราชบัญญัติ (พ.ร.บ.)</b></li>
                                <li><b>การตั้ง/ยุบ/เปลี่ยนเขตอำเภอ:</b> ต้องตราเป็น <b>พระราชกฤษฎีกา (พ.ร.ฎ.)</b></li>
                                <li><b>การปฏิบัติราชการแทน:</b> ผู้มีอำนาจ "มอบอำนาจ" ให้ผู้อื่นทำแทนได้ เพื่อความรวดเร็ว (ผู้มอบยังอยู่)</li>
                                <li><b>การรักษาราชการแทน:</b> เกิดขึ้นเมื่อ "ไม่มีผู้ดำรงตำแหน่ง" หรือมีแต่ปฏิบัติหน้าที่ไม่ได้ (ป่วย, ลา)</li>
                            </ul>
                        </div>
                    </div>
                `
            },
            'good-governance': {
                title: 'พ.ร.ฎ. บริหารกิจการบ้านเมืองที่ดี',
                short_desc: 'คู่มือปฏิบัติงานของข้าราชการ มี 7 เป้าหมายหลัก',
                icon: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#22c55e" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"></path><polyline points="9 22 9 12 15 12 15 22"></polyline></svg>',
                color: 'green',
                details: `
                    <h3 class="text-2xl font-bold text-green-800 mb-4">พ.ร.ฎ. ว่าด้วยหลักเกณฑ์และวิธีการบริหารกิจการบ้านเมืองที่ดี พ.ศ. 2546</h3>
                    <p class="mb-4 text-gray-600">เป็นเหมือนคู่มือปฏิบัติงานของข้าราชการ เพื่อให้การทำงานเกิดประโยชน์สูงสุดต่อประชาชน</p>
                    <div>
                        <h4 class="font-semibold text-lg text-green-700">🎯 7 เป้าหมายหลัก (ต้องจำ!)</h4>
                        <ol class="list-decimal list-inside mt-2 text-gray-600 space-y-1">
                            <li><b>เกิดประโยชน์สุขของประชาชน:</b> ยึดประชาชนเป็นศูนย์กลาง</li>
                            <li><b>เกิดผลสัมฤทธิ์ต่อภารกิจของรัฐ:</b> ทำงานต้องมีแผน (แผน 5 ปี) และเป้าหมายชัดเจน</li>
                            <li><b>มีประสิทธิภาพและเกิดความคุ้มค่า:</b> ใช้ทรัพยากรให้คุ้มค่าที่สุด</li>
                            <li><b>ไม่มีขั้นตอนการปฏิบัติงานเกินความจำเป็น:</b> ลดขั้นตอน ลดเวลา ลดค่าใช้จ่าย</li>
                            <li><b>มีการปรับปรุงภารกิจของส่วนราชการ:</b> ทบทวนภารกิจให้ทันสมัยอยู่เสมอ</li>
                            <li><b>ประชาชนได้รับการอำนวยความสะดวก:</b> จัดตั้ง "ศูนย์บริการร่วม" และใช้ "แพลตฟอร์มดิจิทัลกลาง"</li>
                            <li><b>มีการประเมินผลการปฏิบัติราชการอย่างสม่ำเสมอ:</b> มีคณะผู้ประเมินอิสระมาตรวจสอบ</li>
                        </ol>
                    </div>
                    <div class="mt-4">
                        <h4 class="font-semibold text-lg text-green-700">🔑 ประเด็นน่าจำ</h4>
                        <ul class="list-disc list-inside mt-2 text-gray-600 space-y-1">
                            <li>หากประชาชนติดต่อสอบถามเป็นหนังสือ ต้องตอบกลับภายใน <b>15 วัน</b></li>
                            <li>การจัดทำแพลตฟอร์มดิจิทัลกลาง ต้องเสร็จใน <b>90 วัน</b> และส่วนราชการต้องนำไปใช้ให้เสร็จใน <b>2 ปี</b></li>
                        </ul>
                    </div>
                `
            },
            'admin-procedure': {
                title: 'พ.ร.บ. วิธีปฏิบัติฯ ปกครอง',
                short_desc: 'ขั้นตอนการออก "คำสั่งทางปกครอง" เพื่อความเป็นธรรม',
                icon: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#facc15" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 20h9"></path><path d="M16.5 3.5a2.121 2.121 0 0 1 3 3L7 19l-4 1 1-4L16.5 3.5z"></path></svg>',
                color: 'yellow',
                details: `
                    <h3 class="text-2xl font-bold text-yellow-800 mb-4">พ.ร.บ. วิธีปฏิบัติราชการทางปกครอง พ.ศ. 2539</h3>
                    <p class="mb-4 text-gray-600">วางกรอบขั้นตอนการทำงานของเจ้าหน้าที่ในการออก "คำสั่งทางปกครอง" (เช่น การออกใบอนุญาต, การอนุมัติ, การสั่งพักงาน) เพื่อให้เกิดความเป็นธรรมและตรวจสอบได้</p>
                    <div class="space-y-4">
                        <div>
                            <h4 class="font-semibold text-lg text-yellow-700">🎯 หลักการสำคัญ</h4>
                            <ul class="list-disc list-inside mt-2 text-gray-600 space-y-1">
                                <li><b>เจ้าหน้าที่ต้องเป็นกลาง:</b> ห้ามพิจารณาเรื่องที่ตนมีส่วนได้เสีย เช่น เป็นคู่กรณีเอง, เป็นญาติ, เป็นเจ้าหนี้/ลูกหนี้</li>
                                <li><b>คู่กรณีมีสิทธิ:</b> สามารถแต่งตั้งทนาย, ขอดูเอกสาร, โต้แย้งและแสดงพยานหลักฐานได้</li>
                                <li><b>รูปแบบคำสั่ง:</b> อาจเป็นหนังสือหรือวาจาก็ได้ แต่ต้องชัดเจน และถ้าเป็นหนังสือต้องให้เหตุผลประกอบ</li>
                                <li><b>ผลของคำสั่ง:</b> มีผลนับแต่คู่กรณีได้รับแจ้ง</li>
                            </ul>
                        </div>
                        <div>
                            <h4 class="font-semibold text-lg text-yellow-700">🔑 ประเด็นน่าจำ</h4>
                            <ul class="list-disc list-inside mt-2 text-gray-600 space-y-1">
                                <li>การยื่นอุทธรณ์คำสั่งทางปกครอง ต้องทำเป็นหนังสือยื่นต่อเจ้าหน้าที่ผู้ทำคำสั่ง ภายใน <b>15 วัน</b> นับแต่วันที่ได้รับแจ้งคำสั่ง</li>
                                <li>การขอให้พิจารณาคดีใหม่ (กรณีมีหลักฐานใหม่) ต้องยื่นภายใน <b>90 วัน</b> นับแต่ที่รู้ถึงเหตุ</li>
                            </ul>
                        </div>
                    </div>
                `
            },
             'ethics': {
                title: 'พ.ร.บ. มาตรฐานทางจริยธรรม',
                short_desc: 'กรอบความประพฤติ 7 ข้อ',
                icon: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#a855f7" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"></polygon></svg>',
                color: 'purple',
                details: `
                    <h3 class="text-2xl font-bold text-purple-800 mb-4">พ.ร.บ. มาตรฐานทางจริยธรรม พ.ศ. 2562</h3>
                    <p class="mb-4 text-gray-600">กำหนดมาตรฐานกลางเพื่อให้เจ้าหน้าที่รัฐทุกคนประพฤติตนอย่างมีคุณธรรม</p>
                    <div>
                        <h4 class="font-semibold text-lg text-purple-700">🎯 7 มาตรฐานทางจริยธรรม (ต้องจำ!)</h4>
                        <ol class="list-decimal list-inside mt-2 text-gray-600 space-y-1">
                           <li><b>ยึดมั่น</b>ในสถาบันหลักของประเทศ (ชาติ ศาสนา พระมหากษัตริย์)</li>
                           <li><b>ซื่อสัตย์สุจริต</b> มีจิตสำนึกที่ดี และรับผิดชอบต่อหน้าที่</li>
                           <li><b>กล้าตัดสินใจ</b>และกระทำในสิ่งที่ถูกต้องชอบธรรม</li>
                           <li><b>คิดถึงประโยชน์ส่วนรวม</b>มากกว่าประโยชน์ส่วนตัว และมีจิตสาธารณะ</li>
                           <li><b>มุ่งผลสัมฤทธิ์</b>ของงาน</li>
                           <li><b>ปฏิบัติหน้าที่อย่างเป็นธรรม</b>และไม่เลือกปฏิบัติ</li>
                           <li><b>ดำรงตนเป็นแบบอย่างที่ดี</b>และรักษาภาพลักษณ์ของทางราชการ</li>
                        </ol>
                    </div>
                     <div class="mt-4">
                        <h4 class="font-semibold text-lg text-purple-700">🔑 ประเด็นน่าจำ</h4>
                         <p class="mt-2 text-gray-600"><b>คณะกรรมการมาตรฐานทางจริยธรรม (ก.ม.จ.)</b> มีหน้าที่กำกับดูแล และต้องทบทวนมาตรฐานทางจริยธรรมนี้ <b>ทุก 5 ปี</b></p>
                    </div>
                `
            },
            'tort': {
                title: 'พ.ร.บ. ความรับผิดทางละเมิด',
                short_desc: 'ใครรับผิดชอบเมื่อเกิดความเสียหาย',
                icon: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#ec4899" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path></svg>',
                color: 'pink',
                details: `
                     <h3 class="text-2xl font-bold text-pink-800 mb-4">พ.ร.บ. ความรับผิดทางละเมิดของเจ้าหน้าที่ พ.ศ. 2539</h3>
                    <p class="mb-4 text-gray-600">กำหนดผู้รับผิดชอบกรณีเจ้าหน้าที่ปฏิบัติหน้าที่แล้วเกิดความเสียหายต่อผู้อื่น</p>
                    <div class="space-y-4">
                        <div>
                            <h4 class="font-semibold text-lg text-pink-700">🎯 หลักการสำคัญ</h4>
                            <ul class="list-disc list-inside mt-2 text-gray-600 space-y-1">
                                <li><b>กรณีที่ 1: เจ้าหน้าที่ทำละเมิด "ในการปฏิบัติหน้าที่"</b>
                                    <ul class="list-inside ml-4">
                                        <li><b>ผู้รับผิดชอบ:</b> หน่วยงานของรัฐ (เช่น กระทรวง, กรม)</li>
                                        <li><b>ผู้เสียหาย:</b> ต้องฟ้อง "หน่วยงานของรัฐ" <b>ห้ามฟ้องเจ้าหน้าที่โดยตรง</b></li>
                                    </ul>
                                </li>
                                <li><b>กรณีที่ 2: เจ้าหน้าที่ทำละเมิด "ที่ไม่เกี่ยวกับการปฏิบัติหน้าที่" (เรื่องส่วนตัว)</b>
                                     <ul class="list-inside ml-4">
                                        <li><b>ผู้รับผิดชอบ:</b> เจ้าหน้าที่ต้องรับผิดชอบเป็นการส่วนตัว</li>
                                        <li><b>ผู้เสียหาย:</b> ต้องฟ้อง "เจ้าหน้าที่" โดยตรง</li>
                                    </ul>
                                </li>
                            </ul>
                        </div>
                        <div>
                            <h4 class="font-semibold text-lg text-pink-700">🔑 ประเด็นน่าจำ</h4>
                            <ul class="list-disc list-inside mt-2 text-gray-600 space-y-1">
                               <li>หน่วยงานจะเรียกเงินคืน (ไล่เบี้ย) จากเจ้าหน้าที่ได้ ก็ต่อเมื่อเจ้าหน้าที่กระทำโดย <b>"จงใจ"</b> หรือ <b>"ประมาทเลินเล่ออย่างร้ายแรง"</b> เท่านั้น</li>
                               <li>การเรียกเงินคืนจะคำนึงถึงความร้ายแรงและความเป็นธรรม โดยให้รับผิดชอบ <b>เฉพาะส่วนของตน</b> (ไม่ใช้หลักลูกหนี้ร่วม)</li>
                            </ul>
                        </div>
                    </div>
                `
            },
            'criminal-code': {
                title: 'ประมวลกฎหมายอาญา',
                short_desc: 'โทษทางอาญาเมื่อทุจริต',
                icon: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#6366f1" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>',
                color: 'indigo',
                details: `
                    <h3 class="text-2xl font-bold text-indigo-800 mb-4">ประมวลกฎหมายอาญา (ความผิดต่อตำแหน่งหน้าที่ราชการ)</h3>
                    <p class="mb-4 text-gray-600">กำหนดโทษทางอาญาสำหรับเจ้าพนักงานที่ทุจริตหรือปฏิบัติหน้าที่โดยมิชอบ</p>
                    <div>
                        <h4 class="font-semibold text-lg text-indigo-700">🎯 มาตราสำคัญที่ออกสอบบ่อย</h4>
                        <ul class="list-disc list-inside mt-2 text-gray-600 space-y-2">
                            <li><b>ม.147 เจ้าพนักงานยักยอกทรัพย์:</b> เบียดบังทรัพย์ที่ตนมีหน้าที่ดูแลรักษาไปเป็นของตนเอง</li>
                            <li><b>ม.149 เจ้าพนักงานเรียก รับ หรือยอมจะรับสินบน:</b> รับผลประโยชน์เพื่อจะทำหรือไม่ทำอะไรในตำแหน่งโดยมิชอบ</li>
                            <li><b>ม.157 เจ้าพนักงานปฏิบัติหรือละเว้นการปฏิบัติหน้าที่โดยมิชอบ/โดยทุจริต:</b> เป็นมาตราที่ครอบคลุมการกระทำผิดของเจ้าหน้าที่อย่างกว้างขวางที่สุด และถูกใช้บ่อยที่สุด</li>
                        </ul>
                    </div>
                `
            },
            'governance-principles': {
                title: 'หลักธรรมาภิบาล',
                short_desc: 'หลักการบริหารจัดการที่ดี 6 ประการ',
                icon: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#f97316" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="8" r="7"></circle><polyline points="8.21 13.89 7 23 12 17 17 23 15.79 13.88"></polyline></svg>',
                color: 'orange',
                details: `
                    <h3 class="text-2xl font-bold text-orange-800 mb-4">หลักธรรมาภิบาล (Good Governance)</h3>
                    <p class="mb-4 text-gray-600">คือหลักการบริหารจัดการที่ดี เป็นแนวคิดสากลที่ช่วยสร้างความน่าเชื่อถือให้องค์กร</p>
                    <div>
                        <h4 class="font-semibold text-lg text-orange-700">🎯 6 หลักการ</h4>
                        <ul class="list-disc list-inside mt-2 text-gray-600 space-y-2">
                            <li><b>หลักนิติธรรม:</b> ทำตามกฎหมายอย่างเท่าเทียม เป็นธรรม</li>
                            <li><b>หลักคุณธรรม:</b> ยึดมั่นในความดีงาม ซื่อสัตย์สุจริต</li>
                            <li><b>หลักความโปร่งใส:</b> เปิดเผยข้อมูล ตรวจสอบได้</li>
                            <li><b>หลักการมีส่วนร่วม:</b> เปิดโอกาสให้ผู้มีส่วนได้เสียเข้ามามีส่วนร่วมตัดสินใจ</li>
                            <li><b>หลักความรับผิดชอบ:</b> ตระหนักในหน้าที่และพร้อมรับผิดต่อผลการกระทำ</li>
                            <li><b>หลักความคุ้มค่า:</b> บริหารทรัพยากรให้เกิดประโยชน์สูงสุดแก่ส่วนรวม</li>
                        </ul>
                    </div>
                `
            }
        };

        // --- APP STATE ---
        let currentPage = 'home';
        let currentLaw = null;

        // --- RENDER FUNCTIONS ---
        const app = document.getElementById('app');

        function renderHomePage() {
            let cardsHtml = Object.keys(laws).map(key => {
                const law = laws[key];
                return `
                    <div onclick="navigateTo('${key}')" class="bg-white p-6 rounded-2xl shadow-sm border border-gray-200 cursor-pointer card-hover">
                        <div class="flex items-center gap-4 mb-3">
                            <div class="flex-shrink-0 w-12 h-12 rounded-lg bg-${law.color}-100 flex items-center justify-center">
                                ${law.icon}
                            </div>
                            <div>
                                <h2 class="text-lg font-semibold text-gray-800">${law.title}</h2>
                            </div>
                        </div>
                        <p class="text-gray-500 text-sm">${law.short_desc}</p>
                    </div>
                `;
            }).join('');

            app.innerHTML = `
                <div class="fade-in">
                    <header class="text-center mb-8 md:mb-12">
                        <h1 class="text-4xl md:text-5xl font-bold text-gray-800">สรุปกฎหมายข้าราชการที่ดี</h1>
                        <p class="text-gray-500 mt-2 text-lg">เลือกหัวข้อที่สนใจเพื่อดูรายละเอียด</p>
                    </header>
                    <main class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                        ${cardsHtml}
                    </main>
                </div>
            `;
        }

        function renderDetailPage(lawKey) {
            const law = laws[lawKey];
            if (!law) {
                renderHomePage();
                return;
            }

            app.innerHTML = `
                <div class="fade-in">
                    <header class="mb-8">
                        <button onclick="navigateTo('home')" class="bg-gray-200 hover:bg-gray-300 text-gray-700 font-bold py-2 px-4 rounded-lg inline-flex items-center transition-colors">
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="mr-2"><line x1="19" y1="12" x2="5" y2="12"></line><polyline points="12 19 5 12 12 5"></polyline></svg>
                            กลับหน้าหลัก
                        </button>
                    </header>
                    <main class="bg-white p-6 md:p-8 rounded-2xl shadow-lg border border-gray-200">
                        ${law.details}
                    </main>
                </div>
            `;
        }

        // --- NAVIGATION ---
        function navigateTo(page, lawKey = null) {
            currentPage = page;
            currentLaw = lawKey;
            window.scrollTo(0, 0); // Scroll to top on page change
            render();
        }

        function render() {
            if (currentPage === 'home') {
                renderHomePage();
            } else {
                renderDetailPage(currentPage);
            }
        }

        // --- INITIAL RENDER ---
        render();

    </script>
</body>
</html>
