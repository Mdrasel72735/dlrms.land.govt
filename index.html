<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>বিআরএস খতিয়ান জেনারেটর</title>
    <link href="https://fonts.googleapis.com/css2?family=Hind+Siliguri:wght@400;500;600;700&display=swap" rel="stylesheet">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Hind Siliguri', 'SolaimanLipi', Arial, sans-serif; }
        body { background-color: #0f172a; color: #fff; padding: 20px; }
        
        .container { max-width: 1050px; margin: auto; }
        .card { background: #1e293b; border: 1px solid #334155; border-radius: 8px; padding: 20px; margin-bottom: 20px; }
        .header-title { font-size: 20px; color: #f97316; margin-bottom: 15px; font-weight: bold; }
        
        .form-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(180px, 1fr)); gap: 10px; }
        .form-group { display: flex; flex-direction: column; gap: 4px; }
        .form-group label { font-size: 13px; color: #cbd5e1; }
        input, select, textarea { background: #0f172a; border: 1px solid #475569; color: #fff; padding: 6px 8px; border-radius: 4px; font-size: 13px; outline: none; }
        input:focus { border-color: #38bdf8; }
        
        .btn-print { background: #16a34a; color: #fff; border: none; padding: 12px 24px; font-size: 16px; font-weight: bold; border-radius: 6px; cursor: pointer; width: 100%; margin-top: 15px; transition: 0.2s; }
        .btn-print:hover { background: #15803d; }

        /* Output Sheet Style */
        .sheet-container { background: #fff; color: #000; padding: 30px 40px; border-radius: 4px; max-width: 1000px; margin: auto; }
        
        .sheet-header { position: relative; margin-bottom: 10px; }
        .khatian-title { text-align: center; font-size: 24px; font-weight: bold; margin-bottom: 10px; }
        .page-no { position: absolute; right: 0; top: 0; font-size: 14px; }
        
        .top-meta { display: flex; justify-content: space-between; font-size: 15px; font-weight: bold; margin-bottom: 8px; }
        
        /* Table Structure */
        .khatian-table { width: 100%; border-collapse: collapse; margin-top: 5px; }
        .khatian-table th, .khatian-table td { border: 1px solid #000; padding: 4px 6px; font-size: 13px; text-align: center; vertical-align: top; }
        .khatian-table th { font-weight: bold; background-color: #f8fafc; }
        .text-left { text-align: left !important; }

        .footer-section { display: flex; justify-content: space-between; align-items: flex-end; margin-top: 15px; position: relative; }
        .footer-text { font-size: 12px; line-height: 1.5; }
        
        /* Official Seal */
        .official-seal {
            width: 90px; height: 90px; border: 2px dashed #0b4928; border-radius: 50%;
            display: flex; flex-direction: column; align-items: center; justify-content: center;
            text-align: center; font-size: 9px; font-weight: bold; color: #0b4928;
            margin: auto;
        }

        @media print {
            body { background: #fff; padding: 0; }
            .no-print { display: none !important; }
            .sheet-container { padding: 0; width: 100%; max-width: 100%; }
            @page { size: A4 landscape; margin: 12mm; }
        }
    </style>
</head>
<body>

<div class="container">
    <!-- Form Controls -->
    <div class="card no-print">
        <div class="header-title">বিআরএস খতিয়ান তথ্য ইনপুট ফরম</div>
        
        <div class="form-grid">
            <div class="form-group"><label>খতিয়ান নং:</label><input type="text" id="in_khatian" value="৬১৮" oninput="updateSheet()"></div>
            <div class="form-group"><label>বিভাগ:</label><input type="text" id="in_division" value="চট্টগ্রাম" oninput="updateSheet()"></div>
            <div class="form-group"><label>জেলা:</label><input type="text" id="in_district" value="নোয়াখালী" oninput="updateSheet()"></div>
            <div class="form-group"><label>উপজেলা/থানা:</label><input type="text" id="in_upazila" value="বেগমগঞ্জ" oninput="updateSheet()"></div>
            <div class="form-group"><label>মৌজা:</label><input type="text" id="in_mouza" value="অনন্তপুর" oninput="updateSheet()"></div>
            <div class="form-group"><label>জে. এল. নং:</label><input type="text" id="in_jl" value="২৩৪" oninput="updateSheet()"></div>
            <div class="form-group"><label>রে. সা. নং:</label><input type="text" id="in_resa" value="" oninput="updateSheet()"></div>
        </div>

        <button class="btn-print" onclick="window.print()">🖨 খতিয়ান সেভ ও প্রিন্ট করুন</button>
    </div>

    <!-- Realistic Output Khatian Document -->
    <div class="sheet-container">
        <div class="sheet-header">
            <div class="page-no">পৃষ্ঠা নং: ১ এর ১</div>
            <div class="khatian-title">খতিয়ান নং- <span id="out_khatian">৬১৮</span></div>
        </div>

        <div class="top-meta">
            <div>বিভাগ: <span id="out_division">চট্টগ্রাম</span></div>
            <div>জেলা: <span id="out_district">নোয়াখালী</span></div>
            <div>উপজেলা/থানা: <span id="out_upazila">বেগমগঞ্জ</span></div>
            <div>মৌজা: <span id="out_mouza">অনন্তপুর</span></div>
            <div>জে. এল. নং: <span id="out_jl">২৩৪</span></div>
            <div>রে. সা. নং: <span id="out_resa"></span></div>
        </div>

        <table class="khatian-table">
            <thead>
                <tr>
                    <th rowspan="2" style="width: 22%;">মালিক, অকৃষি প্রজা বা ইজারাদারের নাম ও ঠিকানা</th>
                    <th rowspan="2" style="width: 6%;">অংশ</th>
                    <th rowspan="2" style="width: 5%;">রাজস্ব</th>
                    <th rowspan="2" style="width: 6%;">দাগ</th>
                    <th rowspan="2" style="width: 8%;">জমি শ্রেণী</th>
                    <th colspan="2" style="width: 12%;">দাগের মোট পরিমাণ</th>
                    <th rowspan="2" style="width: 9%;">দাগের মধ্যে অত্র খতিয়ানের অংশ</th>
                    <th colspan="2" style="width: 12%;">অংশানুযায়ী জমির পরিমাণ</th>
                    <th rowspan="2" style="width: 20%;">দখল বিষয়ক বা অন্যান্য বিশেষ মন্তব্য</th>
                </tr>
                <tr>
                    <th>একর</th><th>শতাংশ</th>
                    <th>একর</th><th>শতাংশ</th>
                </tr>
                <tr>
                    <th>১</th><th>২</th><th>৩</th><th>৪</th><th>৫</th><th>৬(ক)</th><th>৬(খ)</th><th>৭</th><th>৮(ক)</th><th>৮(খ)</th><th>৯</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td class="text-left" style="line-height: 1.4;">
                        <b>মালিক:</b><br>
                        দং-গিয়াস উদ্দিন - ০.১২৫<br>
                        নিজাম উদ্দিন - ০.১২৫<br>
                        মহি উদ্দিন - ০.১২৫<br>
                        কামাল উদ্দিন - ০.১২৫<br>
                        সিরাজ উদ্দিন - ০.১২৫<br>
                        আলা উদ্দিন - ০.১২৫<br>
                        জহির উদ্দিন - ০.১২৫<br>
                        শাাফিয়া খাতুন জং আনোয়ার আহমেদ - ০.০৭৫<br>
                        মনোয়ারা বেগম জং ফজলুল হক - ০.০৫০<br>
                        সাং নিজ
                    </td>
                    <td><br>১.০০০</td>
                    <td></td>
                    <td>৪২৫৭<br>৪২৫৮<br>৪২৫৯</td>
                    <td>বাড়ী<br>বাড়ী<br>বাড়ী</td>
                    <td><br><br>১</td>
                    <td>৫৮.০০<br>১৮.০০<br>০০.০০</td>
                    <td>০.১০৩<br>০.০৫৫<br>০.৩০০</td>
                    <td>০<br>০<br>০</td>
                    <td>০৬.০০<br>০১.০০<br>৩০.০০</td>
                    <td class="text-left">
                        টিন/১<br>
                        টিন/১ ঘর/১<br>
                    </td>
                </tr>
                <tr>
                    <td class="text-left"><b>মোট জমি:</b></td>
                    <td><b>১.০০০</b></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td></td>
                    <td><b>০</b></td>
                    <td><b>৩৭.০০</b></td>
                    <td></td>
                </tr>
            </tbody>
        </table>

        <div class="footer-section">
            <div class="footer-text">
                মুদ্রণ: সেটলেমেন্ট প্রেস, ঢাকা। তারিখ: ২৬-০৮-২০২৬<br>
                বাংলাদেশ ফরম নং ৫৪৬২ (সংশোধিত)
            </div>

            <div class="official-seal">
                উপজেলা রেকর্ড রুম<br>
                জেলা প্রশাসকের<br>
                কার্যালয়<br>
                নোয়াখালী
            </div>

            <div id="qrcode"></div>
        </div>
    </div>
</div>

<script>
    function updateSheet() {
        document.getElementById('out_khatian').innerText = document.getElementById('in_khatian').value;
        document.getElementById('out_division').innerText = document.getElementById('in_division').value;
        document.getElementById('out_district').innerText = document.getElementById('in_district').value;
        document.getElementById('out_upazila').innerText = document.getElementById('in_upazila').value;
        document.getElementById('out_mouza').innerText = document.getElementById('in_mouza').value;
        document.getElementById('out_jl').innerText = document.getElementById('in_jl').value;
        document.getElementById('out_resa').innerText = document.getElementById('in_resa').value;
        generateQR();
    }

    function generateQR() {
        const qrContainer = document.getElementById('qrcode');
        qrContainer.innerHTML = '';
        
        const khatian = document.getElementById('in_khatian').value;
        const division = document.getElementById('in_division').value;
        const district = document.getElementById('in_district').value;
        const upazila = document.getElementById('in_upazila').value;
        const mouza = document.getElementById('in_mouza').value;

        const verifyURL = `https://mdrasel72735.github.io/land-verify/verify.html?khatian=${encodeURIComponent(khatian)}&division=${encodeURIComponent(division)}&district=${encodeURIComponent(district)}&upazila=${encodeURIComponent(upazila)}&mouza=${encodeURIComponent(mouza)}&owner=${encodeURIComponent('দং-গিয়াস উদ্দিন ও অন্যান্য')}&dag=${encodeURIComponent('৪২৫৭, ৪২৫৮, ৪২৫৯')}`;

        new QRCode(qrContainer, {
            text: verifyURL,
            width: 75,
            height: 75
        });
    }

    window.onload = function() {
        generateQR();
    };
</script>

</body>
</html>
