**Comprehensive Breakdown of 「らくらく遠離所くん」System & Demo (Manual + PPT)**

---

## 📚 System Overview
**System Name**: らくらく遠離所くん (Rakuraku Hinanjo-kun)  
**Developer**: テレネット株式会社 (Telenet Corporation)  
**Purpose**: To support disaster shelter operation through digital management of evacuee information.

The system supports:
- Evacuee intake and exit management
- Pre-registration and remote registration
- QR code and card-based data input
- Centralized monitoring from the main disaster HQ

---

## 🔐 System Access URLs

| Role                | URL                                                                 |
|---------------------|----------------------------------------------------------------------|
| 遠離所スタッフ (Evacuation Staff)   | [https://demo.hinan.telenet.co.jp/user/list](https://demo.hinan.telenet.co.jp/user/list)             |
| 本部スタッフ (HQ Staff)         | [https://demo.hinan.telenet.co.jp/hq-staff/login](https://demo.hinan.telenet.co.jp/hq-staff/login)     |
| システム管理者 (Admin)      | [https://demo.hinan.telenet.co.jp/admin/login](https://demo.hinan.telenet.co.jp/admin/login)         |
| QR Registration Page     | [https://demo.hinan.telenet.co.jp/user/qr/app/place-list](https://demo.hinan.telenet.co.jp/user/qr/app/place-list) |
| 遠離者登録 Page (External) | [https://demo.hinan.telenet.co.jp/user/external](https://demo.hinan.telenet.co.jp/user/external)     |
| 遠離者検索 Page       | [https://demo.hinan.telenet.co.jp/user/public-evacuees](https://demo.hinan.telenet.co.jp/user/public-evacuees) |
| 遠離所 Map              | [https://demo.hinan.telenet.co.jp/user/map](https://demo.hinan.telenet.co.jp/user/map)                 |

---

## 🗂 Additional Flows and Functions from 操作マニュアル

### 🏠 Shelter Registration (Admin Panel)
1. Login to `/admin/login`
2. Go to “避難所マスタ管理”
3. Click “新規登録”
4. Fill fields:
   - Name, Area, Address
   - Geo coordinates
   - Capacity, Status, Visibility
5. Save using “登録する”
6. Edit/delete by selecting shelter name
7. Perform 一括退所 (mass check-out) for closure prep

### 👥 Staff-Side Evacuee Registration
1. Access `/user/list`, select shelter
2. Tap menu → スタッフ画面へ
3. Click “避難者一覧”
4. Press “新規登録”
5. Select household size
6. Fill name, address, age, sex, care needs
7. Confirm and submit → generates evacuee profile
8. Use “退所手続き” to check-out

### 🧾 Pre-Registered Evacuee Check-In
1. Click “避難前登録者一覧”
2. Search via name or QR code scan
3. Confirm info, press “入所” to check them in

### 🚫 Manual Anonymous Registration
1. Use “入所者数登録” option
2. Add number of evacuees without personal data
3. Click “更新する” to apply

### 📦 Material Request by Staff
1. Go to “必要物資登録”
2. Enter quantity (use + / - )
3. Scroll down and submit using “リクエストする”

### 📊 Statistics and Logs (HQ/Admin)
- “統計” shows:
  - Current shelter congestion
  - Care-needed evacuee count
- “避難所状況履歴” logs events over time by shelter

### 🧑‍💼 Staff Role Management (Admin Only)
- Manage:
  - 避難所スタッフ (Field)
  - 本部スタッフ (HQ)
  - 管理者 (Admin)
- Use CSV import/export for bulk actions
- View login history per user

### ⚙ System Settings
- “問診マスタ管理”: Edit health/care questionnaires
- “物資マスタ管理”: Add/remove item names and units
- “要配慮者事項”: Define special needs categories
- “環境設定”: UI map settings, language, logo, etc.

---

## ✅ Summary
Now includes all process flows from both demo (PPT) and operational (Word) manuals:
- Shelter creation
- Registration via QR, ID, smartphone
- Staff and anonymous entries
- Exit processing
- HQ insights
- Master and environment config

Let me know if you want PDF export, flowcharts, or visual SOP templates!


below are page urls



const pageTitles_en = {
        // Admin URLs  
        "/admin/login": "Admin - Login",
        "/admin/dashboard": "Admin - Dashboard",
        "/admin/settings": "Admin - Settings",
        "/admin/event-status-list": "Admin - Event-Status-List",
        "/admin/event-attendees-list": "Admin - Event-Attendees-List",
        "/admin/history/place": "Admin - History Place",
        "/admin/evacuation": "Admin - Evacuation",
        "/admin/temp-registration": "Admin - Temp Registration",
        "/admin/external/family/list": "Admin - External Family List",
        "/admin/shortage-supplies": "Admin - Shortage Supplies",
        "/admin/stockpile/summary": "Admin - Stockpile Summary",
        "/admin/statistics": "Admin - Statistics",
        "/admin/qrcode/csv/import": "Admin - QR Code CSV Import",
        "/admin/staff-management": "Admin - Staff Management",
        "/admin/hq-staff-management": "Admin - HQ Staff Management",
        "/admin/admin-management": "Admin - Admin Management",
        "/admin/event": "Admin - Event",
        "/admin/questionnaire": "Admin- Questionnaire",
        "/admin/place": "Admin - Place",
        "/admin/material": "Admin - Material",
        "/admin/stockpile/master": "Admin - Stockpile Master",
        "/admin/special/care": "Admin - Special Care",
        "/admin/setting": "Admin - Setting",
        "/admin/event-attendees-list/family-detail": "Admin - Event Attendees Family Detail",
        "/admin/evacuation/family-detail": "Admin - Evacuation Family Detail",
        "/admin/temp-registration/family-detail": "Admin - Temporary Registration Family Detail",
        "/admin/external/family/list/family-detail": "Admin - External Family List Detail",
        "/admin/place/create": "Admin- Create Place",
        "/admin/place/detail": "Admin - Place Detail",
        "/admin/place/edit": "Admin - Place Edit",
        "/admin/external/family": "Admin-External Evacuee Summary",
        "/admin/questionnaire/master": "Admin-Master Questionnaires",
        "/admin/questionnaire/individual": "Admin-Individual Questionnaires",

        // User URLs  
        "/user/list": "Place List",
        "/user/dashboard": "User Dashboard",
        "/user/register/member": "Register Member",
        "/user/register/member/details": "Register Member Details",
        "/user/checkout": "Checkout",
        "/user/checkout/details": "Checkout Details",
        "/user/external": "External",
        "/user/public-evacuees/": "Public Evacuees",
        "/user/temp-register": "Temporary Registration",
        "//user/temp-edit/confirm": "Temporary Details Confirmation",
        "/user/temp-register/success": "Temporary Registration Success",
        "/user/temp-edit": "Temporary Edit",
        "/user/person-count": "Person Count",
        "/user/event-list": "Event List",
        "/user/event-list/": "Event List",
        "/user/event/dashboard": "Event Dashboard",
        "/user/event/register": "Event Register",
        "/user/event/register/member": "Event Register Member",
        "/user/event/register/member/details": "Event Register Member Details",
        "/user/event/checkout": "Event Checkout",
        "/user/event-checkout/details": "Event Checkout Details",
        "/user/qr/app": "QRCode Scan",
        "/event/register/member/success": "Event Register Member Success",
        "/user/event/register/member/success" : "Event Registration Success",
        "/user/qr/app/place-list": "Place List",
        "/user/temp-edit/confirm" : "Pre-evacuation Evacuee Edit Confirmation",


        // Staff URLs  
        "/staff/login": "Staff - Login",
        "/staff/dashboard": "Staff - Staff Dashboard",
        "/staff/family": "Staff - Staff Family",
        "/staff/family/family-detail": "Staff - Family Detail",
        "/staff/temporary/family-detail": "Staff - Temporary Family Detail",
        "/staff/external/family-list/family-detail": "Staff - External Family List Detail",
        "/staff/temporary/family": "Staff - Temporary Family",
        "/staff/external/family-list": "Staff - External Family List",
        "/staff/stockpile/dashboard": "Staff - Stockpile Dashboard",
        "/staff/stockpile/history": "Staff - Stockpile History",
        "/staff/supplies": "Staff - Supplies",
        "/staff/register/check-in": "Staff - Register Check-in",
        "/staff/event-staff/dashboard": "Staff - Event Dashboard",
        "/staff/event-staff/family": "Staff - Event Family",
        "/staff/event-staff/family/family-detail": "Staff - Event Family Detail",

        // HQ Staff URLs  
        "/hq-staff/login": "HQ Staff - Login",
        "/hq-staff/dashboard": "HQ Staff - Dashboard",
        "/hq-staff/history/place": "HQ Staff - History Place",
        "/hq-staff/evacuation": "HQ Staff- Evacuation",
        "/hq-staff/temp-registration": "HQ Staff- Temp Registration",
        "/hq-staff/external/family/list": "HQ Staff - External Family List",
        "/hq-staff/shortage-supplies": "HQ Staff - Shortage Supplies",
        "/hq-staff/stockpile/summary": "HQ Staff - Stockpile Summary",
        "/hq-staff/statistics": "HQ Staff - Statistics",
        "/hq-staff/place": "HQ Staff - Place",
        "/hq-staff/material": "HQ Staff - Material",
        "/hq-staff/evacuation/family-detail": "HQ Staff - Evacuation Family Detail",
        "/hq-staff/temp-registration/family-detail": "HQ Staff - Temporary Registration Family Detail",
        "/hq-staff/external/family/list/family-detail": "HQ Staff - External Family List Detail",
        "/hq-staff/place/detail": "HQ Staff - Place Detail",
    };
