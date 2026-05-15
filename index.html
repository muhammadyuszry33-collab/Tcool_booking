# Tcool_booking
Calender booking for tcool
<!DOCTYPE html>
<html lang="ms">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TCOOL Aircond Enterprise | Sistem Tempahan Rasmi</title>
    
    <!-- Library CSS & JS -->
    <link href="https://cdn.jsdelivr.net/npm/fullcalendar@6.1.15/index.global.min.css" rel="stylesheet">
    <script src="https://cdn.jsdelivr.net/npm/fullcalendar@6.1.15/index.global.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root { --primary: #0a3d62; --secondary: #3c6382; --accent: #ffc107; --success: #25d366; }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Roboto, sans-serif; }
        body { background-color: #f4f7f6; padding: 15px; }
        .container { max-width: 1100px; margin: auto; }

        /* Header Korporat */
        .header { 
            background: linear-gradient(135deg, var(--primary), var(--secondary)); 
            color: white; padding: 35px 20px; border-radius: 20px; 
            margin-bottom: 25px; text-align: center; box-shadow: 0 8px 20px rgba(0,0,0,0.1); 
        }
        .header h1 { font-size: 2.2rem; margin-bottom: 8px; font-weight: 800; }
        .header p { opacity: 0.9; font-size: 1rem; font-weight: 300; }

        /* Layout Grid */
        .main-layout { display: grid; grid-template-columns: 1fr; gap: 25px; }
        @media (min-width: 900px) { .main-layout { grid-template-columns: 1.1fr 0.9fr; } }

        /* Kad Section */
        .card { background: white; padding: 25px; border-radius: 20px; box-shadow: 0 4px 15px rgba(0,0,0,0.05); border: 1px solid #eef0f2; }
        .card-title { font-size: 1.25rem; color: var(--primary); margin-bottom: 20px; font-weight: 700; border-bottom: 2px solid #f8f9fa; padding-bottom: 12px; display: flex; align-items: center; gap: 10px; }

        /* Kalendar UI */
        #calendar { background: #fff; border-radius: 12px; }
        .fc .fc-toolbar-title { font-size: 1.2rem !important; font-weight: 700; color: var(--primary); }
        .fc .fc-button-primary { background-color: var(--primary); border: none; border-radius: 8px; }
        .fc .fc-daygrid-day.fc-day-today { background-color: #fff9db !important; }

        /* Slot Masa */
        .slots-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(110px, 1fr)); gap: 12px; margin-top: 15px; }
        .slot-btn { padding: 12px; border: 2px solid #edeff0; border-radius: 12px; text-align: center; cursor: pointer; transition: 0.3s; font-size: 0.95rem; font-weight: 600; background: #fafafa; }
        .slot-btn:hover { border-color: var(--accent); background: #fffdf5; }
        .slot-btn.active { background: var(--primary); color: white; border-color: var(--primary); }

        /* Borang Input */
        .form-group { margin-bottom: 18px; }
        label { display: block; margin-bottom: 7px; font-weight: 600; font-size: 0.9rem; color: #555; }
        input, select, textarea { width: 100%; padding: 13px 16px; border: 1.5px solid #e0e0e0; border-radius: 12px; font-size: 1rem; transition: 0.3s; background: #fefefe; }
        input:focus, select:focus, textarea:focus { border-color: var(--primary); outline: none; box-shadow: 0 0 0 4px rgba(10, 61, 98, 0.1); }

        /* Ringkasan */
        .summary-box { background: #f8f9fa; padding: 20px; border-radius: 15px; border-left: 6px solid var(--accent); margin: 20px 0; }
        .summary-box p { font-size: 0.95rem; margin-bottom: 8px; color: #444; }
        .price-display { font-size: 1.5rem; color: #2ecc71; font-weight: 800; display: block; margin-top: 5px; }

        /* Butang WhatsApp */
        .btn-whatsapp { 
            width: 100%; padding: 20px; background: var(--success); color: white; border: none; 
            border-radius: 50px; font-size: 1.15rem; font-weight: 700; cursor: pointer; 
            display: flex; align-items: center; justify-content: center; gap: 12px; 
            transition: 0.3s; box-shadow: 0 10px 20px rgba(37, 211, 102, 0.2); 
        }
        .btn-whatsapp:hover { background: #1ebd5b; transform: translateY(-3px); box-shadow: 0 15px 25px rgba(37, 211, 102, 0.3); }

        footer { text-align: center; margin-top: 40px; color: #888; font-size: 0.85rem; padding-bottom: 20px; }
    </style>
</head>
<body>

<div class="container">
    <!-- Header -->
    <div class="header">
        <h1><i class="fas fa-snowflake"></i> TCOOL AIRCOND</h1>
        <p>Professional Air Conditioning Services | Booking System</p>
    </div>

    <div class="main-layout">
        <!-- Bahagian Kalendar & Slot -->
        <div class="card">
            <div class="card-title"><i class="fas fa-calendar-alt"></i> 1. Pilih Tarikh & Masa</div>
            <div id="calendar"></div>
            
            <div style="margin-top: 25px;">
                <label><i class="fas fa-clock"></i> Pilih Slot Masa Tersedia:</label>
                <div id="timeSlotsGrid" class="slots-grid">
                    <div style="grid-column: 1/-1; text-align: center; padding: 20px; color: #aaa;">Sila klik pada tarikh kalendar dahulu.</div>
                </div>
            </div>
        </div>

        <!-- Bahagian Borang -->
        <div class="card">
            <div class="card-title"><i class="fas fa-edit"></i> 2. Maklumat Perkhidmatan</div>
            
            <div class="form-group">
                <label>Nama Penuh Pelanggan</label>
                <input type="text" id="custName" placeholder="Masukkan nama anda">
            </div>

            <div class="form-group">
                <label>Alamat Lengkap (Lokasi Servis)</label>
                <textarea id="custAddress" rows="2" placeholder="No rumah, jalan, taman, poskod"></textarea>
            </div>

            <div class="form-group">
                <label>Jenis Perkhidmatan</label>
                <select id="serviceType">
                    <option value="Normal Service" data-price="80">Normal Service (RM80/unit)</option>
                    <option value="Chemical Service" data-price="150">Chemical Service (RM150/unit)</option>
                    <option value="Overhaul Service" data-price="250">Overhaul Service (RM250/unit)</option>
                    <option value="Checking / Repair" data-price="50">Checking & Repair (Mulai RM50)</option>
                    <option value="New Installation" data-price="250">Installation (Mulai RM250)</option>
                </select>
            </div>

            <div class="summary-box">
                <p><i class="fas fa-calendar-day"></i> Tarikh: <strong id="valDate">-</strong></p>
                <p><i class="fas fa-user-clock"></i> Masa: <strong id="valTime">-</strong></p>
                <p><i class="fas fa-tags"></i> Anggaran Harga: <span class="price-display" id="valPrice">RM 0.00</span></p>
            </div>

            <button class="btn-whatsapp" onclick="submitBooking()">
                <i class="fab fa-whatsapp"></i> Sahkan & Hantar Tempahan
            </button>
        </div>
    </div>

    <footer>
        &copy; 2025 TCOOL AIRCOND ENTERPRISE. All Rights Reserved.
    </footer>
</div>

<script>
    let selectedDate = "";
    let selectedTime = "";
    const whatsappNumber = "601161606431"; // Nombor anda sudah siap sedia

    document.addEventListener('DOMContentLoaded', function() {
        const calendarEl = document.getElementById('calendar');
        const calendar = new FullCalendar.Calendar(calendarEl, {
            initialView: 'dayGridMonth',
            height: 'auto',
            selectable: true,
            dateClick: function(info) {
                selectedDate = info.dateStr;
                document.getElementById('valDate').innerText = selectedDate;
                generateSlots();
                updateTotal();
                
                // Scroll ke slot masa untuk mobile
                if(window.innerWidth < 768) {
                    document.getElementById('timeSlotsGrid').scrollIntoView({ behavior: 'smooth' });
                }
            }
        });
        calendar.render();
    });

    function generateSlots() {
        const grid = document.getElementById('timeSlotsGrid');
        const slots = ["09:00 AM", "11:00 AM", "02:00 PM", "04:00 PM", "08:00 PM"];
        grid.innerHTML = "";
        
        slots.forEach(time => {
            const btn = document.createElement('div');
            btn.className = "slot-btn";
            btn.innerText = time;
            btn.onclick = function() {
                document.querySelectorAll('.slot-btn').forEach(b => b.classList.remove('active'));
                btn.classList.add('active');
                selectedTime = time;
                document.getElementById('valTime').innerText = time;
            };
            grid.appendChild(btn);
        });
    }

    function updateTotal() {
        const select = document.getElementById('serviceType');
        const price = select.options[select.selectedIndex].getAttribute('data-price');
        document.getElementById('valPrice').innerText = "RM " + price + ".00";
    }

    document.getElementById('serviceType').addEventListener('change', updateTotal);

    function submitBooking() {
        const name = document.getElementById('custName').value.trim();
        const address = document.getElementById('custAddress').value.trim();
        const service = document.getElementById('serviceType').value;
        const price = document.getElementById('valPrice').innerText;

        if(!selectedDate || !selectedTime || !name || !address) {
            Swal.fire({
                icon: 'error',
                title: 'Maklumat Tidak Lengkap',
                text: 'Sila pilih tarikh, slot masa, dan isi semua maklumat anda.',
                confirmButtonColor: '#0a3d62'
            });
            return;
        }

        // Format mesej untuk WhatsApp
        const msg = `*TEMPAHAN SERVIS TCOOL AIRCOND*%0A` +
                    `-----------------------------------%0A` +
                    `*Nama:* ${name}%0A` +
                    `*Tarikh:* ${selectedDate}%0A` +
                    `*Masa:* ${selectedTime}%0A` +
                    `*Servis:* ${service}%0A` +
                    `*Alamat:* ${address}%0A` +
                    `*Anggaran:* ${price}%0A` +
                    `-----------------------------------%0A` +
                    `Sila sahkan tempahan saya. Terima kasih!`;

        const finalUrl = `https://wa.me/${whatsappNumber}?text=${msg}`;
        
        Swal.fire({
            title: 'Hantar Tempahan?',
            text: "Anda akan dibawa ke WhatsApp untuk pengesahan akhir.",
            icon: 'question',
            showCancelButton: true,
            confirmButtonColor: '#25d366',
            cancelButtonColor: '#d33',
            confirmButtonText: 'Ya, Hantar Sekarang!'
        }).then((result) => {
            if (result.isConfirmed) {
                window.open(finalUrl, '_blank');
            }
        });
    }
</script>

</body>
</html>
