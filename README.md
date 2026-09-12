<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>Dragon Mart Weekly Staff Roster</title>

<style>
*{
    box-sizing:border-box;
}

body{
    margin:0;
    font-family:Segoe UI,Arial,sans-serif;
    background:#fff;
}

/* ================= LOGIN ================= */

#loginPage{
    position:fixed;
    inset:0;
    z-index:99999;
    display:flex;
    align-items:center;
    justify-content:center;
    padding:20px;
    background:
        radial-gradient(circle at top right,#d99a2b 0%,transparent 35%),
        linear-gradient(135deg,#151515,#292929,#111);
}

.login-card{
    width:100%;
    max-width:430px;
    background:#fff;
    border-radius:20px;
    padding:35px 32px;
    text-align:center;
    box-shadow:0 20px 50px rgba(0,0,0,.35);
}

.login-logo{
    width:110px;
    height:110px;
    margin:auto;
    display:flex;
    align-items:center;
    justify-content:center;
}

.login-logo img{
    max-width:105px;
    max-height:105px;
    object-fit:contain;
}

.login-card h1{
    margin:0;
    font-size:30px;
    color:#222;
}

.login-card h2{
    margin:5px 0 8px;
    font-size:21px;
    color:#555;
}

.login-subtitle{
    color:#777;
    font-size:14px;
    margin-bottom:25px;
}

.login-field{
    text-align:left;
    margin-bottom:18px;
}

.login-field label{
    display:block;
    margin-bottom:7px;
    font-weight:700;
    font-size:14px;
}

.login-field input{
    width:100%;
    padding:13px;
    border:1px solid #ccc;
    border-radius:9px;
    font-size:15px;
}

.pass-box{
    position:relative;
}

.pass-box input{
    padding-right:45px;
}

.show-pass{
    position:absolute;
    right:5px;
    top:50%;
    transform:translateY(-50%);
    border:0;
    background:transparent;
    cursor:pointer;
    font-size:17px;
}

.login-button{
    width:100%;
    padding:14px;
    border:0;
    border-radius:9px;
    background:linear-gradient(135deg,#6a11cb,#2575fc);
    color:white;
    font-size:16px;
    font-weight:700;
    cursor:pointer;
}

.login-error{
    min-height:20px;
    margin-top:14px;
    color:#dc3545;
    font-size:13px;
    font-weight:600;
}

.login-footer{
    margin-top:25px;
    padding-top:18px;
    border-top:1px solid #eee;
    color:#999;
    font-size:12px;
}

/* ================= APP ================= */

#app{
    display:none;
    padding:20px;
}

.header{
    height:150px;
    display:flex;
    align-items:center;
    justify-content:center;
    position:relative;
}

.logo{
    position:absolute;
    left:10px;
    top:0;
    width:170px;
    height:150px;
    display:flex;
    align-items:center;
    justify-content:center;
}

.logo img{
    max-width:160px;
    max-height:140px;
    object-fit:contain;
}

.title{
    font-size:28px;
    font-weight:bold;
    color:#222;
    text-shadow:1px 1px 2px #aaa;
}

.week{
    text-align:center;
    font-size:18px;
    font-weight:bold;
    color:#444;
    margin:5px 0 15px;
}

.controls,
.week-controls{
    text-align:center;
    margin:12px 0;
}

button.action{
    border:0;
    border-radius:6px;
    padding:10px 18px;
    margin:5px;
    color:#fff;
    font-size:14px;
    font-weight:600;
    cursor:pointer;
}

.prev{background:#6c757d}
.next{background:#007bff}
.save{background:#28a745}
.print{background:#007bff}
.csv{background:#6f42c1}
.image{background:#17a2b8}
.add{background:#20c997}

/* ================= TABLE ================= */

table{
    width:100%;
    border-collapse:collapse;
    table-layout:fixed;
    background:#fff;
    box-shadow:0 4px 8px rgba(0,0,0,.1);
}

th,
td{
    border:1px solid #d0d0d0;
    padding:8px 4px;
    text-align:center;
    vertical-align:middle;
    font-size:13px;
}

th{
    background:linear-gradient(135deg,#6a11cb,#2575fc);
    color:#fff;
    font-weight:700;
}

th:first-child,
td:first-child{
    width:180px;
}

.name-input{
    width:95%;
    padding:8px;
    border:1px solid #bbb;
    border-radius:5px;
    text-align:center;
    font-size:14px;
    font-weight:700;
    color:#222;
}

select{
    width:100%;
    max-width:145px;
    padding:8px 3px;
    border-radius:6px;
    border:2px solid #aaa;
    font-size:12px;
    font-weight:700;
    cursor:pointer;
}

/* ================= FINAL SHIFT COLORS ================= */

.AM{
    background:#FFD54F!important;
    color:#5D4037!important;
    border:2px solid #FBC02D!important;
}

.PM{
    background:#4CAF50!important;
    color:#fff!important;
    border:2px solid #388E3C!important;
}

.Off{
    background:#90CAF9!important;
    color:#0D47A1!important;
    border:2px solid #64B5F6!important;
}

.AL{
    background:#F8D7DA!important;
    color:#721C24!important;
    border:2px solid #E5A1A6!important;
}

.Management{
    background:#FFF2CC!important;
    color:#7F6000!important;
    border:2px solid #FFD966!important;
}

.FS{
    background:#ff9800!important;
    color:#fff!important;
    border:2px solid #ef6c00!important;
    font-weight:800!important;
}

.Custom{
    background:#8D6E63!important;
    color:#fff!important;
    border:2px solid #6D4C41!important;
    font-weight:800!important;
}

.MID{
    background:#CFD8DC!important;
    color:#37474F!important;
    border:2px solid #90A4AE!important;
    font-weight:800!important;
}

.SelectShift{
    background:#fff!important;
    color:#555!important;
    border:2px solid #ccc!important;
}

.duplicate{
    border:3px solid red!important;
    box-shadow:0 0 7px rgba(255,0,0,.7)!important;
}

/* ================= SUMMARY ================= */

.summary td{
    background:#f7f7f7;
    color:#333;
    font-size:11px;
    font-weight:700;
    padding:6px 2px;
}

.summary td:first-child{
    background:#eee;
}

/* ================= SHIFT TIMING ================= */

.shift-timing{
    margin:18px 0 10px;
    border:1px solid #d6d6d6;
    border-radius:8px;
    overflow:hidden;
    background:#fff;
    box-shadow:0 3px 7px rgba(0,0,0,.08);
}

.shift-timing-title{
    padding:9px;
    text-align:center;
    font-size:15px;
    font-weight:800;
    color:#333;
    background:#f3f3f3;
}

.shift-timing-table{
    width:100%;
    border-collapse:collapse;
    box-shadow:none;
}

.shift-timing-table th,
.shift-timing-table td{
    border:1px solid #ddd;
    padding:7px 5px;
    font-size:12px;
    text-align:center;
}

.shift-timing-table th{
    background:#f7f7f7;
    color:#333;
}

.timing-am{
    background:#FFD54F!important;
    color:#5D4037!important;
    font-weight:800;
}

.timing-pm{
    background:#4CAF50!important;
    color:#fff!important;
    font-weight:800;
}

.timing-mid{
    background:#CFD8DC!important;
    color:#37474F!important;
    font-weight:800;
}

/* ================= MOBILE ================= */

@media(max-width:800px){

    #app{
        padding:8px;
    }

    .header{
        height:110px;
    }

    .logo{
        width:100px;
        height:100px;
    }

    .logo img{
        max-width:90px;
        max-height:90px;
    }

    .title{
        font-size:20px;
    }

    th:first-child,
    td:first-child{
        width:120px;
    }

    th,
    td{
        font-size:10px;
        padding:5px 2px;
    }

    select{
        font-size:10px;
        padding:6px 1px;
    }

    .shift-timing-table th,
    .shift-timing-table td{
        font-size:9px;
        padding:5px 2px;
    }

    .shift-timing-title{
        font-size:13px;
    }
}

/* ================= PRINT ================= */

@media print{

    #loginPage,
    .week-controls,
    .controls{
        display:none!important;
    }

    #app{
        display:block!important;
        padding:10px;
    }

    .AM,
    .PM,
    .Off,
    .AL,
    .Management,
    .FS,
    .Custom,
    .MID,
    .summary td,
    .timing-am,
    .timing-pm,
    .timing-mid{
        -webkit-print-color-adjust:exact!important;
        print-color-adjust:exact!important;
    }
}
</style>
</head>

<body>

<div id="loginPage">

<div class="login-card">

    <div class="login-logo">
        <img
            src="https://th.bing.com/th/id/OIP.-yQulJpK9XsIT5HcBWQgrAHaHZ?w=108&h=108&c=1&bgcl=d69c3b"
            alt="Dragon Mart Logo">
    </div>

    <h1>Dragon Mart</h1>
    <h2>Staff Roster Login</h2>

    <p class="login-subtitle">
        Please sign in to access the weekly roster
    </p>

    <form id="loginForm">

        <div class="login-field">
            <label>Username</label>
            <input
                id="username"
                type="text"
                autocomplete="username"
                placeholder="Enter username"
                required>
        </div>

        <div class="login-field">

            <label>Password</label>

            <div class="pass-box">

                <input
                    id="password"
                    type="password"
                    autocomplete="current-password"
                    placeholder="Enter password"
                    required>

                <button
                    type="button"
                    class="show-pass"
                    onclick="togglePassword()">👁️</button>

            </div>

        </div>

        <button
            class="login-button"
            type="submit">
            🔐 Login
        </button>

        <div
            id="loginError"
            class="login-error">
        </div>

    </form>

    <div class="login-footer">
        Dragon Mart Weekly Staff Roster
    </div>

</div>
</div>


<div id="app">

<div class="header">

    <div class="logo">

        <img
            src="https://th.bing.com/th/id/OIP.-yQulJpK9XsIT5HcBWQgrAHaHZ?w=108&h=108&c=1&bgcl=d69c3b"
            alt="Dragon Mart Logo">

    </div>

    <div class="title">
        Dragon Mart Weekly Staff Roster
    </div>

</div>

<div id="week" class="week"></div>

<div class="week-controls">

    <button
        class="action prev"
        onclick="changeWeek(-1)">
        ⬅️ Previous Week
    </button>

    <button
        class="action save"
        onclick="saveRoster(true)">
        💾 Save Roster
    </button>

    <button
        class="action next"
        onclick="changeWeek(1)">
        Next Week ➡️
    </button>

</div>

<table id="rosterTable"></table>

<!-- ================= SHIFT TIMING / BREAKS ================= -->

<div id="shiftTiming" class="shift-timing"></div>

<div class="controls">

    <button
        class="action print"
        onclick="window.print()">
        🖨️ Print / PDF
    </button>

    <button
        class="action csv"
        onclick="downloadCSV()">
        ⬇️ Download CSV
    </button>

    <button
        class="action image"
        onclick="downloadImage()">
        🖼️ Download Roster as Image
    </button>

    <button
        class="action add"
        onclick="addStaff()">
        ➕ Add Staff
    </button>

</div>

</div>

<script src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js"></script>

<script>

/* =================================================
   LOGIN
================================================= */

const USERNAME = "Dragon Mart";
const PASSWORD = "CSA2026";

document
.getElementById("loginForm")
.addEventListener(
    "submit",
    function(e){

        e.preventDefault();

        const username =
            document.getElementById("username")
            .value
            .trim();

        const password =
            document.getElementById("password")
            .value;

        if(
            username === USERNAME &&
            password === PASSWORD
        ){

            sessionStorage.setItem(
                "DragonMartLoggedIn",
                "true"
            );

            document
            .getElementById("loginError")
            .textContent = "";

            openApp();

        }else{

            document
            .getElementById("loginError")
            .textContent =
                "❌ Incorrect username or password.";
        }

    }
);


function togglePassword(){

    const password =
        document.getElementById("password");

    const button =
        document.querySelector(".show-pass");

    if(password.type === "password"){

        password.type = "text";
        button.textContent = "🙈";

    }else{

        password.type = "password";
        button.textContent = "👁️";
    }
}


function openApp(){

    document
    .getElementById("loginPage")
    .style.display = "none";

    document
    .getElementById("app")
    .style.display = "block";

    loadWeek();
}


/* =================================================
   STAFF
================================================= */

const STAFF = [
    "Marie",
    "Varun",
    "Allaine",
    "Iswary",
    "Aqil",
    "Kim",
    "Aahan",
    "Flora",
    "April",
    "Amine",
    "Saber",
    "Sadaf",
    "Alameen",
    "Anjum",
    "Nourhan",
    "Yasmine",
    "Afrith",
    "Alnoor"
];

const STAFF_STORAGE_KEY =
    "DragonMartRosterPermanentStaff";


function getPermanentStaff(){

    let saved =
        localStorage.getItem(
            STAFF_STORAGE_KEY
        );

    if(saved === null){

        savePermanentStaff(STAFF);
        return [...STAFF];
    }

    try{

        const parsed =
            JSON.parse(saved);

        if(Array.isArray(parsed)){
            return parsed;
        }

    }catch(error){

        console.warn(
            "Could not read permanent staff:",
            error
        );
    }

    savePermanentStaff(STAFF);

    return [...STAFF];
}


function savePermanentStaff(staffList){

    const unique = [];

    staffList.forEach(name => {

        const cleanName =
            String(name).trim();

        if(
            cleanName &&
            !unique.some(
                existing =>
                    existing.toLowerCase() ===
                    cleanName.toLowerCase()
            )
        ){

            unique.push(cleanName);
        }

    });

    localStorage.setItem(
        STAFF_STORAGE_KEY,
        JSON.stringify(unique)
    );
}


/* =================================================
   DESKS
================================================= */

const DESKS = [
    "BA",
    "F",
    "H",
    "GA",
    "GD"
];

const MANAGEMENT = [
    "Iswary",
    "April"
];

const DAYS = [
    "Mon",
    "Tue",
    "Wed",
    "Thu",
    "Fri",
    "Sat",
    "Sun"
];


/* =================================================
   WEEK
================================================= */

let weekNumber = 0;

const FIRST_WEEK =
    new Date(2026,8,14);

const STORAGE_KEY =
    "DragonMartRosterWeek_";


function getStartDate(){

    const date =
        new Date(FIRST_WEEK);

    date.setDate(
        date.getDate() +
        weekNumber * 7
    );

    return date;
}


function formatDate(date){

    return (
        String(date.getDate()).padStart(2,"0")
        + "-"
        +
        String(
            date.getMonth()+1
        ).padStart(2,"0")
        + "-"
        +
        date.getFullYear()
    );
}


/* =================================================
   LOAD WEEK
================================================= */

function loadWeek(){

    const table =
        document.getElementById(
            "rosterTable"
        );

    table.innerHTML = "";

    updateWeekDisplay();
    createHeader();

    let data = null;

    const saved =
        localStorage.getItem(
            STORAGE_KEY + weekNumber
        );

    if(saved){

        try{

            data = JSON.parse(saved);

        }catch(error){

            data = null;
        }
    }

    const permanentStaff =
        getPermanentStaff();

    if(!Array.isArray(data)){

        data =
            permanentStaff.map(name => ({

                name:name,

                days:[
                    "",
                    "",
                    "",
                    "",
                    "",
                    "",
                    ""
                ]

            }));

    }else{

        permanentStaff.forEach(name => {

            const exists =
                data.some(
                    person =>
                        String(person.name)
                        .trim()
                        .toLowerCase() ===
                        name
                        .trim()
                        .toLowerCase()
                );

            if(!exists){

                data.push({

                    name:name,

                    days:[
                        "",
                        "",
                        "",
                        "",
                        "",
                        "",
                        ""
                    ]

                });
            }

        });
    }

    data.forEach(person => {

        addStaffRow(
            person.name,
            person.days
        );

    });

    createSummary();
    updateDuplicate();
    updateSummary();
    updateShiftTiming();
}


/* =================================================
   WEEK DISPLAY
================================================= */

function updateWeekDisplay(){

    const start =
        getStartDate();

    const end =
        new Date(start);

    end.setDate(
        start.getDate() + 6
    );

    document
    .getElementById("week")
    .textContent =
        "Week: " +
        formatDate(start) +
        " - " +
        formatDate(end);
}


/* =================================================
   HEADER
================================================= */

function createHeader(){

    const table =
        document.getElementById(
            "rosterTable"
        );

    const row =
        table.insertRow();

    row.insertCell().outerHTML =
        "<th>Staff Name</th>";

    const start =
        getStartDate();

    DAYS.forEach(
        (day,index) => {

            const date =
                new Date(start);

            date.setDate(
                start.getDate() + index
            );

            row.insertCell().outerHTML =
                `
                <th>
                    ${day}<br>
                    ${formatDate(date)}
                </th>
                `;
        }
    );
}


/* =================================================
   STAFF ROW
================================================= */

function addStaffRow(
    name,
    days
){

    const table =
        document.getElementById(
            "rosterTable"
        );

    const row =
        table.insertRow();

    const nameCell =
        row.insertCell();

    const input =
        document.createElement(
            "input"
        );

    input.className =
        "name-input";

    input.value =
        name || "";

    input.onchange =
        () => saveRoster(false);

    nameCell.appendChild(input);

    for(let day=0;day<7;day++){

        row.insertCell().appendChild(

            makeShiftSelect(
                name,
                days?.[day] || "",
                day
            )

        );
    }
}


/* =================================================
   CUSTOM VALUE
================================================= */

function isCustomValue(value){

    return (
        typeof value === "string" &&
        value.startsWith("CUSTOM::")
    );
}


function getCustomText(value){

    if(!isCustomValue(value))
        return "";

    return value.substring(8);
}


function createCustomValue(text){

    return "CUSTOM::" + text;
}


/* =================================================
   SHIFT SELECT
================================================= */

function makeShiftSelect(
    staffName,
    savedValue,
    day
){

    const select =
        document.createElement(
            "select"
        );

    let html = `

        <option value="">
            Select Shift
        </option>

        <option value="MID">
            MID
        </option>
    `;


    html += DESKS.map(
        desk =>
        `
        <option value="${desk}-AM">
            ${desk} (AM)
        </option>
        `
    ).join("");


    html += DESKS.map(
        desk =>
        `
        <option value="${desk}-PM">
            ${desk} (PM)
        </option>
        `
    ).join("");


    html += DESKS.map(
        desk =>
        `
        <option value="${desk} FS">
            ${desk} (FS)
        </option>
        `
    ).join("");


    if(
        MANAGEMENT.includes(
            staffName
        )
    ){

        html += `

            <option value="Management-AM">
                Management (AM)
            </option>

            <option value="Management-PM">
                Management (PM)
            </option>

        `;
    }


    html += `

        <option value="Off">
            OFF
        </option>

        <option value="AL">
            AL
        </option>

        <option value="CUSTOM">
            CUSTOM
        </option>

    `;

    select.innerHTML = html;


    if(isCustomValue(savedValue)){

        const customText =
            getCustomText(savedValue);

        const customOption =
            document.createElement(
                "option"
            );

        customOption.value =
            savedValue;

        customOption.textContent =
            customText || "CUSTOM";

        customOption.dataset.custom =
            "true";

        select.appendChild(
            customOption
        );
    }


    select.value =
        savedValue || "";

    applyColor(select);


    select.addEventListener(
        "change",
        function(){

            if(
                select.value === "CUSTOM"
            ){

                const customText =
                    prompt(
                        "✏️ Enter your custom option:"
                    );

                if(
                    customText === null ||
                    !customText.trim()
                ){

                    select.value = "";

                    applyColor(select);
                    updateDuplicate();
                    updateSummary();
                    saveRoster(false);

                    return;
                }

                const cleanText =
                    customText.trim();

                const customValue =
                    createCustomValue(
                        cleanText
                    );


                [...select.options]
                .forEach(option => {

                    if(
                        option.dataset.custom ===
                        "true"
                    ){

                        option.remove();
                    }

                });


                const customOption =
                    document.createElement(
                        "option"
                    );

                customOption.value =
                    customValue;

                customOption.textContent =
                    cleanText;

                customOption.dataset.custom =
                    "true";

                select.appendChild(
                    customOption
                );

                select.value =
                    customValue;
            }

            applyColor(select);
            updateDuplicate();
            updateSummary();
            saveRoster(false);

        }
    );

    return select;
}


/* =================================================
   COLORS
================================================= */

function applyColor(select){

    const value =
        select.value;

    select.className = "";


    if(!value){

        select.className =
            "SelectShift";

    }else if(
        value === "MID"
    ){

        select.className =
            "MID";

    }else if(
        value === "Off"
    ){

        select.className =
            "Off";

    }else if(
        value === "AL"
    ){

        select.className =
            "AL";

    }else if(
        isCustomValue(value)
    ){

        select.className =
            "Custom";

    }else if(
        value.startsWith(
            "Management"
        )
    ){

        select.className =
            "Management";

    }else if(
        value.endsWith(" FS")
    ){

        select.className =
            "FS";

    }else if(
        value.endsWith("-AM")
    ){

        select.className =
            "AM";

    }else if(
        value.endsWith("-PM")
    ){

        select.className =
            "PM";
    }
}


/* =================================================
   DUPLICATE
================================================= */

function updateDuplicate(){

    const table =
        document.getElementById(
            "rosterTable"
        );


    [...table.rows]
    .slice(1)
    .forEach(row => {

        if(
            row.classList.contains(
                "summary"
            )
        )
            return;

        row
        .querySelectorAll("select")
        .forEach(select => {

            select.classList.remove(
                "duplicate"
            );

            select.title = "";
        });
    });


    [...table.rows]
    .slice(1)
    .forEach(row => {

        if(
            row.classList.contains(
                "summary"
            )
        )
            return;

        const seen = {};

        row
        .querySelectorAll("select")
        .forEach(select => {

            const value =
                select.value;

            if(!value)
                return;

            if(
                value === "MID" ||
                value === "Off" ||
                value === "AL" ||
                value === "FS" ||
                isCustomValue(value) ||
                value.startsWith(
                    "Management"
                )
            )
                return;

            if(seen[value]){

                select.classList.add(
                    "duplicate"
                );

                select.title =
                    "Duplicate shift in this staff row";

            }else{

                seen[value] = true;
            }

        });

    });


    for(
        let day=0;
        day<7;
        day++
    ){

        const used = {};

        [...table.rows]
        .slice(1)
        .forEach(row => {

            if(
                row.classList.contains(
                    "summary"
                )
            )
                return;

            const select =
                row.cells[day+1]
                ?.querySelector(
                    "select"
                );

            if(!select)
                return;

            const value =
                select.value;

            if(
                value &&
                value !== "MID" &&
                value !== "Off" &&
                value !== "AL" &&
                value !== "FS" &&
                !isCustomValue(value) &&
                !value.startsWith(
                    "Management"
                ) &&
                !value.endsWith(
                    " FS"
                )
            ){

                used[value] = true;
            }

        });


        [...table.rows]
        .slice(1)
        .forEach(row => {

            if(
                row.classList.contains(
                    "summary"
                )
            )
                return;

            const select =
                row.cells[day+1]
                ?.querySelector(
                    "select"
                );

            if(!select)
                return;

            [...select.options]
            .forEach(option => {

                option.disabled = false;

                if(
                    used[option.value] &&
                    option.value !==
                        select.value &&
                    option.value &&
                    option.value !== "MID" &&
                    option.value !== "Off" &&
                    option.value !== "AL" &&
                    option.value !== "FS" &&
                    !isCustomValue(
                        option.value
                    ) &&
                    !option.value.startsWith(
                        "Management"
                    ) &&
                    !option.value.endsWith(
                        " FS"
                    )
                ){

                    option.disabled = true;
                }

            });

        });
    }
}


/* =================================================
   SUMMARY
================================================= */

function createSummary(){

    const table =
        document.getElementById(
            "rosterTable"
        );

    const row =
        table.insertRow();

    row.className =
        "summary";

    row.insertCell().textContent =
        "Daily Summary";

    for(let i=0;i<7;i++){

        row.insertCell();
    }
}


function updateSummary(){

    const table =
        document.getElementById(
            "rosterTable"
        );

    const row =
        table.querySelector(
            ".summary"
        );

    if(!row)
        return;


    for(
        let day=0;
        day<7;
        day++
    ){

        const count = {

            AM:0,
            PM:0,
            OFF:0,
            AL:0,
            MID:0,
            FS:0,
            CUSTOM:0

        };


        [...table.rows]
        .slice(1)
        .forEach(r => {

            if(
                r.classList.contains(
                    "summary"
                )
            )
                return;

            const select =
                r.cells[day+1]
                ?.querySelector(
                    "select"
                );

            if(!select)
                return;

            const value =
                select.value;

            if(value === "MID")
                count.MID++;

            else if(
                value === "Off"
            )
                count.OFF++;

            else if(
                value === "AL"
            )
                count.AL++;

            else if(
                value === "FS" ||
                value.endsWith(" FS")
            )
                count.FS++;

            else if(
                isCustomValue(value)
            )
                count.CUSTOM++;

            else if(
                value.endsWith("-AM")
            )
                count.AM++;

            else if(
                value.endsWith("-PM")
            )
                count.PM++;

        });


        row.cells[day+1].textContent =
            `AM ${count.AM} | ` +
            `PM ${count.PM} | ` +
            `OFF ${count.OFF} | ` +
            `AL ${count.AL} | ` +
            `MID ${count.MID} | ` +
            `FS ${count.FS} | ` +
            `CUSTOM ${count.CUSTOM}`;
    }
}


/* =================================================
   SHIFT TIMING + BREAKS
================================================= */

function getShiftTimingType(){

    const start = getStartDate();

    return start;
}


function updateShiftTiming(){

    const container =
        document.getElementById(
            "shiftTiming"
        );

    if(!container)
        return;

    const start =
        getShiftTimingType();

    const end =
        new Date(start);

    end.setDate(
        start.getDate() + 6
    );

    container.innerHTML = `

        <div class="shift-timing-title">
            ⏰ Shift Timings & Breaks
        </div>

        <table class="shift-timing-table">

            <tr>
                <th>Days</th>
                <th>Shift</th>
                <th>Working Time</th>
                <th>Break</th>
            </tr>

            <tr>
                <td rowspan="3">
                    Sunday – Thursday
                </td>

                <td class="timing-am">
                    AM
                </td>

                <td>
                    10:00 AM – 7:00 PM
                </td>

                <td>
                    1:00 PM – 2:00 PM
                </td>
            </tr>

            <tr>

                <td class="timing-pm">
                    PM
                </td>

                <td>
                    1:00 PM – 10:00 PM
                </td>

                <td>
                    5:00 PM – 6:00 PM
                </td>

            </tr>

            <tr>

                <td class="timing-mid">
                    MID
                </td>

                <td>
                    12:00 PM – 9:00 PM
                </td>

                <td>
                    3:00 PM – 4:00 PM
                </td>

            </tr>

            <tr>
                <td rowspan="3">
                    Friday – Saturday
                </td>

                <td class="timing-am">
                    AM
                </td>

                <td>
                    10:00 AM – 7:00 PM
                </td>

                <td>
                    2:00 PM – 3:00 PM
                </td>
            </tr>

            <tr>

                <td class="timing-pm">
                    PM
                </td>

                <td>
                    2:00 PM – 11:00 PM
                </td>

                <td>
                    5:00 PM – 6:00 PM
                </td>

            </tr>

            <tr>

                <td class="timing-mid">
                    MID
                </td>

                <td>
                    12:00 PM – 9:00 PM
                </td>

                <td>
                    3:00 PM – 4:00 PM
                </td>

            </tr>

        </table>
    `;
}


/* =================================================
   SAVE
================================================= */

function saveRoster(show){

    const table =
        document.getElementById(
            "rosterTable"
        );

    const data = [];


    [...table.rows]
    .slice(1)
    .forEach(row => {

        if(
            row.classList.contains(
                "summary"
            )
        )
            return;

        const input =
            row.cells[0]
            ?.querySelector(
                "input"
            );

        const days = [];

        for(
            let i=1;
            i<=7;
            i++
        ){

            const select =
                row.cells[i]
                ?.querySelector(
                    "select"
                );

            days.push(
                select?.value || ""
            );
        }

        data.push({

            name:
                input?.value || "",

            days:days

        });

    });


    localStorage.setItem(
        STORAGE_KEY + weekNumber,
        JSON.stringify(data)
    );


    const currentPermanentStaff =
        getPermanentStaff();

    const currentNames =
        data
        .map(person =>
            String(person.name).trim()
        )
        .filter(Boolean);

    savePermanentStaff([
        ...currentPermanentStaff,
        ...currentNames
    ]);


    if(show){

        alert(
            "✅ Roster saved successfully!"
        );
    }
}


/* =================================================
   WEEK CHANGE
================================================= */

function changeWeek(amount){

    saveRoster(false);

    weekNumber += amount;

    if(
        weekNumber < 0
    ){

        weekNumber = 0;
    }

    loadWeek();
}


/* =================================================
   ADD / REMOVE STAFF
================================================= */

function addStaff(){

    const choice =
        prompt(
            "👤 Staff Management\n\n" +
            "1 - Add Staff\n" +
            "2 - Remove Staff\n" +
            "3 - Cancel\n\n" +
            "Enter 1, 2 or 3:"
        );


    if(
        choice === null ||
        choice === "3"
    ){

        return;
    }


    if(choice === "1"){

        const name =
            prompt(
                "👤 Enter new staff name:"
            );

        if(name === null)
            return;

        const newName =
            name.trim();

        if(!newName){

            alert(
                "⚠️ Please enter a valid staff name."
            );

            return;
        }


        const table =
            document.getElementById(
                "rosterTable"
            );

        const existing =
            [...table.rows]
            .slice(1)
            .filter(
                row =>
                    !row.classList.contains(
                        "summary"
                    )
            )
            .map(
                row =>
                    row.cells[0]
                    ?.querySelector(
                        "input"
                    )
                    ?.value
                    .trim()
                    .toLowerCase()
            );


        if(
            existing.includes(
                newName.toLowerCase()
            )
        ){

            alert(
                "⚠️ This staff member already exists."
            );

            return;
        }


        const permanentStaff =
            getPermanentStaff();

        const permanentExists =
            permanentStaff.some(
                staff =>
                    staff.toLowerCase() ===
                    newName.toLowerCase()
            );


        if(permanentExists){

            alert(
                "⚠️ This staff member already exists."
            );

            return;
        }


        savePermanentStaff([
            ...permanentStaff,
            newName
        ]);


        const summary =
            table.querySelector(
                ".summary"
            );

        const row =
            table.insertRow(
                summary
                    ? summary.rowIndex
                    : table.rows.length
            );

        const cell =
            row.insertCell();

        const input =
            document.createElement(
                "input"
            );

        input.className =
            "name-input";

        input.value =
            newName;

        input.onchange =
            () => saveRoster(false);

        cell.appendChild(input);


        for(
            let day=0;
            day<7;
            day++
        ){

            row.insertCell().appendChild(

                makeShiftSelect(
                    newName,
                    "",
                    day
                )

            );
        }


        const storageKeys = [];

        for(
            let i=0;
            i<localStorage.length;
            i++
        ){

            const key =
                localStorage.key(i);

            if(
                key &&
                key.startsWith(
                    STORAGE_KEY
                )
            ){

                storageKeys.push(key);
            }
        }


        storageKeys.forEach(key => {

            const savedWeekNumber =
                parseInt(
                    key.replace(
                        STORAGE_KEY,
                        ""
                    ),
                    10
                );


            if(
                !isNaN(savedWeekNumber) &&
                savedWeekNumber > weekNumber
            ){

                try{

                    const weekData =
                        JSON.parse(
                            localStorage.getItem(
                                key
                            )
                        );


                    if(
                        Array.isArray(
                            weekData
                        )
                    ){

                        const exists =
                            weekData.some(
                                person =>
                                    String(
                                        person.name
                                    )
                                    .trim()
                                    .toLowerCase() ===
                                    newName
                                    .toLowerCase()
                            );


                        if(!exists){

                            weekData.push({

                                name:newName,

                                days:[
                                    "",
                                    "",
                                    "",
                                    "",
                                    "",
                                    "",
                                    ""
                                ]

                            });


                            localStorage.setItem(
                                key,
                                JSON.stringify(
                                    weekData
                                )
                            );
                        }
                    }

                }catch(error){

                    console.warn(
                        "Could not update future week:",
                        key,
                        error
                    );
                }
            }

        });


        updateDuplicate();
        updateSummary();
        saveRoster(false);


        alert(
            "✅ " +
            newName +
            " has been added.\n\n" +

            "Current week + future weeks updated.\n" +

            "Past weeks were not changed."
        );

        return;
    }


    if(choice === "2"){

        const permanentStaff =
            getPermanentStaff();


        if(
            permanentStaff.length === 0
        ){

            alert(
                "⚠️ No staff available to remove."
            );

            return;
        }


        const staffList =
            permanentStaff
            .map(
                (staff,index) =>
                    `${index + 1}. ${staff}`
            )
            .join("\n");


        const removeName =
            prompt(
                "🗑️ Remove Staff\n\n" +
                "Current Staff:\n\n" +
                staffList +
                "\n\n" +
                "Enter the staff name to remove:"
            );


        if(removeName === null)
            return;


        const cleanRemoveName =
            removeName.trim();


        if(!cleanRemoveName){

            alert(
                "⚠️ Please enter a staff name."
            );

            return;
        }


        const existingStaff =
            permanentStaff.find(
                staff =>
                    staff.toLowerCase() ===
                    cleanRemoveName.toLowerCase()
            );


        if(!existingStaff){

            alert(
                `❌ "${cleanRemoveName}" was not found in the staff list.`
            );

            return;
        }


        const confirmed =
            confirm(
                `⚠️ Are you sure you want to remove "${existingStaff}"?\n\n` +

                `This will remove the staff member from:\n` +

                `• Current week\n` +
                `• Future weeks\n\n` +

                `Past weeks will NOT be changed.`
            );


        if(!confirmed)
            return;


        const updatedStaff =
            permanentStaff.filter(
                staff =>
                    staff.toLowerCase() !==
                    existingStaff.toLowerCase()
            );


        savePermanentStaff(
            updatedStaff
        );


        const storageKeys = [];

        for(
            let i=0;
            i<localStorage.length;
            i++
        ){

            const key =
                localStorage.key(i);

            if(
                key &&
                key.startsWith(
                    STORAGE_KEY
                )
            ){

                storageKeys.push(key);
            }
        }


        storageKeys.forEach(key => {

            const savedWeekNumber =
                parseInt(
                    key.replace(
                        STORAGE_KEY,
                        ""
                    ),
                    10
                );


            if(
                !isNaN(savedWeekNumber) &&
                savedWeekNumber > weekNumber
            ){

                try{

                    const weekData =
                        JSON.parse(
                            localStorage.getItem(
                                key
                            )
                        );


                    if(
                        Array.isArray(
                            weekData
                        )
                    ){

                        const filtered =
                            weekData.filter(
                                person =>
                                    String(
                                        person.name
                                    )
                                    .trim()
                                    .toLowerCase() !==
                                    existingStaff
                                    .toLowerCase()
                            );


                        localStorage.setItem(
                            key,
                            JSON.stringify(
                                filtered
                            )
                        );
                    }

                }catch(error){

                    console.warn(
                        "Could not update future week:",
                        key,
                        error
                    );
                }
            }

        });


        const table =
            document.getElementById(
                "rosterTable"
            );


        [...table.rows]
        .slice(1)
        .forEach(row => {

            if(
                row.classList.contains(
                    "summary"
                )
            )
                return;

            const input =
                row.cells[0]
                ?.querySelector(
                    "input"
                );


            if(
                input &&
                input.value
                .trim()
                .toLowerCase() ===
                existingStaff
                .toLowerCase()
            ){

                row.remove();
            }

        });


        updateDuplicate();
        updateSummary();
        saveRoster(false);


        alert(
            "✅ " +
            existingStaff +
            " has been removed.\n\n" +

            "Current week + future weeks updated.\n" +

            "Past weeks were NOT changed."
        );

        return;
    }


    alert(
        "❌ Invalid choice.\n\n" +
        "Please enter 1, 2 or 3."
    );
}


/* =================================================
   DISPLAY VALUE
================================================= */

function displayValue(value){

    if(!value)
        return "Select Shift";

    if(value === "Off")
        return "OFF";

    if(value === "MID")
        return "MID";

    if(value === "AL")
        return "AL";

    if(value === "FS")
        return "FS";


    if(
        isCustomValue(value)
    ){

        return getCustomText(value);
    }


    if(
        value.endsWith(" FS")
    ){

        return value.replace(
            " FS",
            " (FS)"
        );
    }


    if(
        value.startsWith(
            "Management-"
        )
    ){

        return (
            "Management (" +
            value.replace(
                "Management-",
                ""
            ) +
            ")"
        );
    }


    if(
        value.endsWith("-AM")
    ){

        return value.replace(
            "-AM",
            " (AM)"
        );
    }


    if(
        value.endsWith("-PM")
    ){

        return value.replace(
            "-PM",
            " (PM)"
        );
    }


    return value;
}


/* =================================================
   CSV
================================================= */

function downloadCSV(){

    saveRoster(false);

    const table =
        document.getElementById(
            "rosterTable"
        );

    const lines = [];


    [...table.rows]
    .forEach(row => {

        const values = [];


        [...row.cells]
        .forEach(cell => {

            const input =
                cell.querySelector(
                    "input"
                );

            const select =
                cell.querySelector(
                    "select"
                );

            let value = "";


            if(input){

                value =
                    input.value;

            }else if(select){

                value =
                    displayValue(
                        select.value
                    );

            }else{

                value =
                    cell.innerText;
            }


            values.push(
                `"${String(value)
                    .replace(
                        /"/g,
                        '""'
                    )
                    .replace(
                        /\s+/g,
                        " "
                    )
                    .trim()}"`
            );

        });


        lines.push(
            values.join(",")
        );

    });


    const blob =
        new Blob(
            [lines.join("\n")],
            {
                type:
                    "text/csv;charset=utf-8"
            }
        );


    downloadBlob(
        blob,
        "Dragon_Mart_Weekly_Roster.csv"
    );
}


/* =================================================
   DOWNLOAD IMAGE
   FIXED:
   LOGO STAYS ON LEFT SIDE
   TITLE STAYS CENTERED
================================================= */

async function downloadImage(){

    saveRoster(false);


    if(
        typeof html2canvas ===
        "undefined"
    ){

        alert(
            "❌ Image library has not loaded yet."
        );

        return;
    }


    const sourceTable =
        document.getElementById(
            "rosterTable"
        );


    const exportBox =
        document.createElement(
            "div"
        );


    exportBox.style.cssText = `

        position:fixed;
        left:-100000px;
        top:0;
        width:1800px;
        padding:30px;
        background:#ffffff;
        font-family:Segoe UI,Arial,sans-serif;
        box-sizing:border-box;

    `;


    /* =================================================
       EXPORT HEADER
       SAME POSITION AS NORMAL HEADER
    ================================================= */

    const exportHeader =
        document.createElement(
            "div"
        );


    exportHeader.style.cssText = `

        position:relative;
        width:100%;
        height:150px;
        display:flex;
        align-items:center;
        justify-content:center;
        box-sizing:border-box;

    `;


    /* ================= LOGO ================= */

    const logoBox =
        document.createElement(
            "div"
        );


    /*
       IMPORTANT:
       Logo is now positioned on the LEFT,
       exactly like the normal .logo section.
    */

    logoBox.style.cssText = `

        position:absolute;
        left:10px;
        top:0;
        width:170px;
        height:150px;
        display:flex;
        align-items:center;
        justify-content:center;

    `;


    const logo =
        document.createElement(
            "img"
        );


    logo.src =
        "https://th.bing.com/th/id/OIP.-yQulJpK9XsIT5HcBWQgrAHaHZ?w=108&h=108&c=1&bgcl=d69c3b";


    logo.alt =
        "Dragon Mart Logo";


    logo.crossOrigin =
        "anonymous";


    logo.style.cssText = `

        max-width:160px;
        max-height:140px;
        width:auto;
        height:auto;
        object-fit:contain;

    `;


    logoBox.appendChild(
        logo
    );


    exportHeader.appendChild(
        logoBox
    );


    /* ================= TITLE ================= */

    const title =
        document.createElement(
            "div"
        );


    title.textContent =
        "Dragon Mart Weekly Staff Roster";


    title.style.cssText = `

        text-align:center;
        font-size:30px;
        font-weight:bold;
        color:#222;
        text-shadow:1px 1px 2px #aaa;
        width:100%;

    `;


    exportHeader.appendChild(
        title
    );


    exportBox.appendChild(
        exportHeader
    );


    /* ================= WEEK ================= */

    const week =
        document.createElement(
            "div"
        );


    week.textContent =
        document.getElementById(
            "week"
        ).textContent;


    week.style.cssText = `

        text-align:center;
        font-size:18px;
        font-weight:bold;
        color:#444;
        margin:5px 0 20px;

    `;


    exportBox.appendChild(
        week
    );


    /* ================= NEW TABLE ================= */

    const table =
        document.createElement(
            "table"
        );


    table.style.cssText = `

        width:100%;
        border-collapse:collapse;
        table-layout:fixed;
        background:#fff;

    `;


    [...sourceTable.rows]
    .forEach(
        sourceRow => {

            const newRow =
                document.createElement(
                    "tr"
                );


            if(
                sourceRow.rowIndex === 0
            ){

                [...sourceRow.cells]
                .forEach(
                    sourceCell => {

                        const cell =
                            document.createElement(
                                "th"
                            );


                        cell.innerHTML =
                            sourceCell.innerHTML;


                        cell.style.cssText = `

                            border:1px solid #aaa;
                            padding:10px 5px;
                            text-align:center;
                            vertical-align:middle;
                            font-size:14px;
                            font-weight:700;
                            color:#fff;
                            background:linear-gradient(
                                135deg,
                                #6a11cb,
                                #2575fc
                            );

                        `;


                        newRow.appendChild(
                            cell
                        );

                    }
                );
            }


            else if(
                sourceRow.classList.contains(
                    "summary"
                )
            ){

                [...sourceRow.cells]
                .forEach(
                    sourceCell => {

                        const cell =
                            document.createElement(
                                "td"
                            );


                        cell.textContent =
                            sourceCell.innerText;


                        cell.style.cssText = `

                            border:1px solid #ccc;
                            padding:8px 3px;
                            text-align:center;
                            vertical-align:middle;
                            font-size:12px;
                            font-weight:700;
                            color:#333;
                            background:#f7f7f7;

                        `;


                        newRow.appendChild(
                            cell
                        );

                    }
                );
            }


            else{

                [...sourceRow.cells]
                .forEach(
                    (sourceCell,index) => {

                        const cell =
                            document.createElement(
                                "td"
                            );


                        cell.style.cssText = `

                            border:1px solid #ccc;
                            padding:7px 4px;
                            text-align:center;
                            vertical-align:middle;
                            font-size:13px;
                            font-weight:700;
                            color:#222;
                            background:#fff;

                        `;


                        if(index === 0){

                            const input =
                                sourceCell
                                .querySelector(
                                    "input"
                                );


                            cell.textContent =
                                input
                                    ? input.value
                                    : sourceCell.innerText;


                            cell.style.fontSize =
                                "15px";


                            cell.style.fontWeight =
                                "700";
                        }


                        else{

                            const select =
                                sourceCell
                                .querySelector(
                                    "select"
                                );


                            const value =
                                select
                                    ? select.value
                                    : "";


                            cell.textContent =
                                displayValue(
                                    value
                                );


                            if(
                                value.endsWith(
                                    "-AM"
                                )
                            ){

                                cell.style.background =
                                    "#FFD54F";

                                cell.style.color =
                                    "#5D4037";

                                cell.style.border =
                                    "2px solid #FBC02D";
                            }


                            else if(
                                value.endsWith(
                                    "-PM"
                                )
                            ){

                                cell.style.background =
                                    "#4CAF50";

                                cell.style.color =
                                    "#fff";

                                cell.style.border =
                                    "2px solid #388E3C";
                            }


                            else if(
                                value === "MID"
                            ){

                                cell.style.background =
                                    "#CFD8DC";

                                cell.style.color =
                                    "#37474F";

                                cell.style.border =
                                    "2px solid #90A4AE";
                            }


                            else if(
                                value === "Off"
                            ){

                                cell.style.background =
                                    "#90CAF9";

                                cell.style.color =
                                    "#0D47A1";

                                cell.style.border =
                                    "2px solid #64B5F6";
                            }


                            else if(
                                value === "AL"
                            ){

                                cell.style.background =
                                    "#F8D7DA";

                                cell.style.color =
                                    "#721C24";

                                cell.style.border =
                                    "2px solid #E5A1A6";
                            }


                            else if(
                                value.startsWith(
                                    "Management"
                                )
                            ){

                                cell.style.background =
                                    "#FFF2CC";

                                cell.style.color =
                                    "#7F6000";

                                cell.style.border =
                                    "2px solid #FFD966";
                            }


                            else if(
                                value === "FS" ||
                                value.endsWith(
                                    " FS"
                                )
                            ){

                                cell.style.background =
                                    "#ff9800";

                                cell.style.color =
                                    "#fff";

                                cell.style.border =
                                    "2px solid #ef6c00";
                            }


                            else if(
                                isCustomValue(value)
                            ){

                                cell.style.background =
                                    "#8D6E63";

                                cell.style.color =
                                    "#fff";

                                cell.style.border =
                                    "2px solid #6D4C41";
                            }


                            else{

                                cell.style.background =
                                    "#fff";

                                cell.style.color =
                                    "#555";

                                cell.style.border =
                                    "1px solid #ccc";
                            }


                            cell.style.minHeight =
                                "42px";

                            cell.style.fontWeight =
                                "800";

                            cell.style.fontSize =
                                "13px";
                        }


                        newRow.appendChild(
                            cell
                        );

                    }
                );
            }


            table.appendChild(
                newRow
            );

        }
    );


    [...table.rows]
    .forEach(row => {

        if(row.cells[0]){

            row.cells[0].style.width =
                "180px";
        }

    });


    exportBox.appendChild(
        table
    );


    /* =================================================
       TIMING SECTION FOR PNG
    ================================================= */

    const timingBox =
        document.createElement(
            "div"
        );


    timingBox.style.cssText = `

        margin-top:18px;
        border:1px solid #d6d6d6;
        border-radius:8px;
        overflow:hidden;
        background:#fff;

    `;


    const timingTitle =
        document.createElement(
            "div"
        );


    timingTitle.textContent =
        "⏰ Shift Timings & Breaks";


    timingTitle.style.cssText = `

        padding:10px;
        text-align:center;
        font-size:16px;
        font-weight:800;
        color:#333;
        background:#f3f3f3;

    `;


    timingBox.appendChild(
        timingTitle
    );


    const timingTable =
        document.createElement(
            "table"
        );


    timingTable.style.cssText = `

        width:100%;
        border-collapse:collapse;
        box-shadow:none;

    `;


    const timingRows = [

        [
            "Days",
            "Shift",
            "Working Time",
            "Break"
        ],

        [
            "Sunday – Thursday",
            "AM",
            "10:00 AM – 7:00 PM",
            "1:00 PM – 2:00 PM"
        ],

        [
            "Sunday – Thursday",
            "PM",
            "1:00 PM – 10:00 PM",
            "5:00 PM – 6:00 PM"
        ],

        [
            "Sunday – Thursday",
            "MID",
            "12:00 PM – 9:00 PM",
            "3:00 PM – 4:00 PM"
        ],

        [
            "Friday – Saturday",
            "AM",
            "10:00 AM – 7:00 PM",
            "2:00 PM – 3:00 PM"
        ],

        [
            "Friday – Saturday",
            "PM",
            "2:00 PM – 11:00 PM",
            "5:00 PM – 6:00 PM"
        ],

        [
            "Friday – Saturday",
            "MID",
            "12:00 PM – 9:00 PM",
            "3:00 PM – 4:00 PM"
        ]

    ];


    timingRows.forEach(
        (rowData,rowIndex) => {

            const row =
                document.createElement(
                    "tr"
                );


            rowData.forEach(
                (text,columnIndex) => {

                    const cell =
                        document.createElement(
                            rowIndex === 0
                                ? "th"
                                : "td"
                        );


                    cell.textContent =
                        text;


                    cell.style.cssText = `

                        border:1px solid #ddd;
                        padding:8px 5px;
                        text-align:center;
                        vertical-align:middle;
                        font-size:12px;
                        font-weight:700;

                    `;


                    if(rowIndex === 0){

                        cell.style.background =
                            "#f7f7f7";

                        cell.style.color =
                            "#333";

                    }else{

                        if(columnIndex === 1){

                            if(text === "AM"){

                                cell.style.background =
                                    "#FFD54F";

                                cell.style.color =
                                    "#5D4037";

                            }else if(text === "PM"){

                                cell.style.background =
                                    "#4CAF50";

                                cell.style.color =
                                    "#fff";

                            }else if(text === "MID"){

                                cell.style.background =
                                    "#CFD8DC";

                                cell.style.color =
                                    "#37474F";
                            }

                        }else{

                            cell.style.background =
                                "#fff";

                            cell.style.color =
                                "#333";
                        }
                    }


                    row.appendChild(
                        cell
                    );

                }
            );


            timingTable.appendChild(
                row
            );

        }
    );


    timingBox.appendChild(
        timingTable
    );


    exportBox.appendChild(
        timingBox
    );


    document.body.appendChild(
        exportBox
    );


    /* =================================================
       WAIT FOR IMAGE / LAYOUT
    ================================================= */

    await new Promise(
        resolve =>
            requestAnimationFrame(
                () =>
                    requestAnimationFrame(
                        resolve
                    )
            )
    );


    try{

        const canvas =
            await html2canvas(
                exportBox,
                {

                    scale:2,

                    backgroundColor:
                        "#ffffff",

                    useCORS:true,

                    allowTaint:false,

                    logging:false,

                    width:
                        exportBox.scrollWidth,

                    height:
                        exportBox.scrollHeight,

                    windowWidth:
                        exportBox.scrollWidth,

                    windowHeight:
                        exportBox.scrollHeight

                }
            );


        canvas.toBlob(
            function(blob){

                if(!blob){

                    alert(
                        "❌ Could not create image."
                    );

                    return;
                }


                downloadBlob(
                    blob,
                    "Dragon_Mart_Weekly_Roster.png"
                );


                alert(
                    "✅ Roster image downloaded successfully!"
                );

            },
            "image/png"
        );


    }catch(error){

        console.error(error);

        alert(
            "❌ Could not create the roster image."
        );

    }finally{

        exportBox.remove();
    }
}


/* =================================================
   DOWNLOAD HELPER
================================================= */

function downloadBlob(
    blob,
    name
){

    const url =
        URL.createObjectURL(
            blob
        );


    const link =
        document.createElement(
            "a"
        );


    link.href = url;

    link.download = name;


    document.body.appendChild(
        link
    );


    link.click();

    link.remove();


    setTimeout(
        () =>
            URL.revokeObjectURL(
                url
            ),
        1000
    );
}


/* =================================================
   AUTO LOGIN
================================================= */

if(
    sessionStorage.getItem(
        "DragonMartLoggedIn"
    ) === "true"
){

    openApp();
}

</script>

</body>
</html>
