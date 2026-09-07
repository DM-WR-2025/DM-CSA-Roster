<html lang="en">

<head>

<meta charset="UTF-8">

<meta name="viewport"
      content="width=device-width, initial-scale=1.0">

<title>Dragon Mart Weekly Staff Roster</title>

<style>

/* =====================================================
   PAGE
===================================================== */

body {

    font-family:
        "Segoe UI",
        Arial,
        sans-serif;

    background: #ffffff;

    padding: 0;

    margin: 0;

    min-height: 100vh;

}


/* =====================================================
   LOGIN PAGE
===================================================== */

#loginPage {

    position: fixed;

    top: 0;
    left: 0;
    right: 0;
    bottom: 0;

    width: 100vw;
    height: 100vh;

    z-index: 99999;

    display: flex;

    align-items: center;

    justify-content: center;

    box-sizing: border-box;

    padding: 20px;

    margin: 0;

    background:
        radial-gradient(
            circle at top right,
            #d99a2b 0%,
            transparent 35%
        ),
        linear-gradient(
            135deg,
            #151515 0%,
            #292929 50%,
            #111111 100%
        );

}


/* LOGIN CARD */

.login-card {

    width: 100%;

    max-width: 430px;

    margin: 0 auto;

    background: #ffffff;

    border-radius: 20px;

    padding: 35px 32px;

    box-sizing: border-box;

    text-align: center;

    box-shadow:
        0 20px 50px
        rgba(0,0,0,.35);

}

.login-card {

    width: 100%;

    max-width: 430px;

    background: #ffffff;

    border-radius: 20px;

    padding: 35px 32px;

    box-sizing: border-box;

    text-align: center;

    box-shadow:
        0 20px 50px
        rgba(0,0,0,.25);

    animation:
        loginFadeIn .45s ease;

}


@keyframes loginFadeIn {

    from {

        opacity: 0;

        transform:
            translateY(20px)
            scale(.97);

    }

    to {

        opacity: 1;

        transform:
            translateY(0)
            scale(1);

    }

}


.login-logo {

    width: 110px;

    height: 110px;

    margin: 0 auto 12px;

    display: flex;

    align-items: center;

    justify-content: center;

}


.login-logo img {

    max-width: 105px;

    max-height: 105px;

    width: auto;

    height: auto;

    object-fit: contain;

}


.login-card h1 {

    margin: 0;

    font-size: 30px;

    color: #222222;

    font-weight: 800;

}


.login-card h2 {

    margin: 5px 0 8px;

    font-size: 21px;

    color: #555555;

}


.login-subtitle {

    margin: 0 0 25px;

    color: #777777;

    font-size: 14px;

}


.login-field {

    text-align: left;

    margin-bottom: 18px;

}


.login-field label {

    display: block;

    margin-bottom: 7px;

    font-size: 14px;

    font-weight: 700;

    color: #333333;

}


.login-field input {

    width: 100%;

    padding: 13px 14px;

    box-sizing: border-box;

    border: 1px solid #cccccc;

    border-radius: 9px;

    font-size: 15px;

    outline: none;

    transition: .25s;

}


.login-field input:focus {

    border-color: #2575fc;

    box-shadow:
        0 0 0 3px
        rgba(37,117,252,.15);

}


.password-wrapper {

    position: relative;

}


.password-wrapper input {

    padding-right: 48px;

}


.show-password {

    position: absolute;

    right: 5px;

    top: 50%;

    transform: translateY(-50%);

    border: none;

    background: transparent;

    padding: 8px;

    cursor: pointer;

    font-size: 17px;

}


.login-button {

    width: 100%;

    border: none;

    border-radius: 9px;

    padding: 14px;

    margin-top: 5px;

    background:
        linear-gradient(
            135deg,
            #6a11cb,
            #2575fc
        );

    color: white;

    font-size: 16px;

    font-weight: 700;

    cursor: pointer;

    transition: .25s;

}


.login-button:hover {

    transform: translateY(-2px);

    box-shadow:
        0 7px 18px
        rgba(37,117,252,.3);

}


.login-error {

    min-height: 20px;

    margin-top: 14px;

    color: #dc3545;

    font-size: 13px;

    font-weight: 600;

}


.login-footer {

    margin-top: 25px;

    padding-top: 18px;

    border-top:
        1px solid #eeeeee;

    color: #999999;

    font-size: 12px;

}


@media (max-width: 480px) {

    .login-card {

        padding: 30px 22px;

    }

    .login-card h1 {

        font-size: 26px;

    }

}


/* =====================================================
   ROSTER AREA
===================================================== */

#rosterArea {

    background: #ffffff;

    padding: 20px;

    box-sizing: border-box;

}


/* =====================================================
   HEADER
===================================================== */

.header {

    display: flex;

    align-items: center;

    justify-content: center;

    margin-bottom: 10px;

    position: relative;

    min-height: 150px;

}


/* =====================================================
   LOGO
===================================================== */

.logo-container {

    position: absolute;

    left: 10px;

    top: 0;

    width: 170px;

    height: 150px;

    display: flex;

    align-items: center;

    justify-content: center;

}


.logo-container img {

    max-height: 140px;

    max-width: 160px;

    width: auto;

    height: auto;

    object-fit: contain;

}


/* =====================================================
   TITLE
===================================================== */

h2 {

    text-align: center;

    margin: 0;

    font-size: 28px;

    color: #222222;

    font-weight: bold;

    text-shadow:
        1px 1px 2px #aaaaaa;

}


/* =====================================================
   WEEK DATE DISPLAY
===================================================== */

.week-display {

    text-align: center;

    font-size: 18px;

    font-weight: bold;

    color: #444444;

    margin: 5px 0 15px 0;

}


/* =====================================================
   WEEK NAVIGATION
===================================================== */

.week-controls {

    text-align: center;

    margin: 10px 0 15px 0;

}


.week-controls button {

    padding: 10px 18px;

    margin: 5px;

    font-size: 14px;

    border: none;

    cursor: pointer;

    color: white;

    border-radius: 6px;

    font-weight: 600;

}


.previous-button {

    background: #6c757d;

}


.next-button {

    background: #007bff;

}


.save-week-button {

    background: #28a745;

}


.week-controls button:hover {

    opacity: .9;

    transform: scale(1.05);

}


/* =====================================================
   BUTTONS
===================================================== */

.controls {

    margin: 15px 0;

    text-align: center;

}


.controls button {

    padding: 10px 18px;

    margin: 5px;

    font-size: 14px;

    border: none;

    cursor: pointer;

    background: #007bff;

    color: white;

    border-radius: 6px;

    transition: .3s;

}


.controls button:hover {

    opacity: .9;

    transform: scale(1.05);

}


.csv-button {

    background: #6f42c1 !important;

}


.image-button {

    background: #17a2b8 !important;

}


.add-staff-button {

    background: #20c997 !important;

}


/* =====================================================
   TABLE
===================================================== */

table {

    width: 100%;

    border-collapse: separate;

    border-spacing: 0;

    background: white;

    border-radius: 8px;

    overflow: hidden;

    box-shadow:
        0 4px 8px
        rgba(0,0,0,.1);

    table-layout: fixed;

}


th,
td {

    border: 1px solid #d5d5d5;

    padding: 9px 5px;

    text-align: center;

    font-size: 14px;

    vertical-align: middle;

}


/* =====================================================
   HEADER CELLS
===================================================== */

th {

    background:
        linear-gradient(
            135deg,
            #6a11cb,
            #2575fc
        );

    color: white;

    font-weight: 600;

    font-size: 14px;

    text-shadow:
        1px 1px 2px
        rgba(0,0,0,.3);

}


/* =====================================================
   STAFF NAME COLUMN
===================================================== */

th:first-child,
td:first-child {

    width: 180px;

    min-width: 180px;

}


td:first-child {

    height: 55px;

}


td:first-child input {

    width: 100%;

    max-width: 165px;

    padding: 8px;

    text-align: center;

    border-radius: 5px;

    border: 1px solid #bbb;

    box-sizing: border-box;

    font-size: 15px;

    font-weight: 700;

    color: #222222;

}


/* =====================================================
   SELECT
===================================================== */

select {

    display: block;

    margin: 0 auto;

    text-align: center;

    width: 100%;

    max-width: 135px;

    padding: 8px 4px;

    border-radius: 6px;

    border: 1px solid #aaa;

    cursor: pointer;

    font-size: 13px;

    font-weight: 600;

}


.SelectShift {

    background: #ffffff !important;

    color: #555555 !important;

    border:
        2px solid #cccccc !important;

}


.AM {

    background:
        #2196F3 !important;

    color: white !important;

    border:
        2px solid #1976D2 !important;

    font-weight: bold;

}


.PM {

    background:
        #4CAF50 !important;

    color: white !important;

    border:
        2px solid #388E3C !important;

    font-weight: bold;

}


.MID {

    background:
        #A0522D !important;

    color: white !important;

    border:
        2px solid #7B3F21 !important;

    font-weight: bold;

}


.Off {

    background:
        #F8D7DA !important;

    color:
        #721C24 !important;

    border:
        2px solid #E5A1A6 !important;

    font-weight: bold;

}


.AL {

    background:
        #9C27B0 !important;

    color: white !important;

    border:
        2px solid #7B1FA2 !important;

    font-weight: bold;

}


.Management {

    background:
        #FFF3CD !important;

    color:
        #856404 !important;

    border:
        2px solid #FFDA6A !important;

    font-weight: bold;

}


.duplicate {

    border:
        3px solid red !important;

    box-shadow:
        0 0 6px
        rgba(255,0,0,.6);

}


/* =====================================================
   REMOVE BUTTON
===================================================== */

td button {

    background:
        #dc3545;

    padding:
        6px 10px;

    border-radius:
        5px;

    color: white;

    border: none;

    cursor: pointer;

}


/* =====================================================
   DAILY SUMMARY
===================================================== */

.summary-row td {

    background: #f7f7f7;

    color: #333333;

    font-size: 11px;

    font-weight: 700;

    padding: 6px 3px;

    line-height: 1.35;

}


.summary-row td:first-child {

    background: #eeeeee;

    color: #555555;

    font-size: 11px;

}


/* =====================================================
   SUMMARY COLORS
===================================================== */

.summary-am {

    color: #1976D2;

}


.summary-pm {

    color: #388E3C;

}


.summary-off {

    color: #b4232c;

}


.summary-al {

    color: #7B1FA2;

}


.summary-mid {

    color: #7B3F21;

}


.summary-management {

    color: #E91E63;

}


/* =====================================================
   PRINT
===================================================== */

@media print {

    #loginPage {

        display: none !important;

    }

    .week-controls {

        display: none;

    }

    .controls {

        display: none;

    }

    body {

        padding: 0;

    }

    #rosterArea {

        padding: 10px;

    }

    .AM,
    .PM,
    .MID,
    .Off,
    .AL,
    .Management {

        -webkit-print-color-adjust:
            exact;

        print-color-adjust:
            exact;

    }

    .summary-row td {

        -webkit-print-color-adjust:
            exact;

        print-color-adjust:
            exact;

    }

}

</style>

</head>


<body>


<!-- =====================================================
     LOGIN PAGE
===================================================== -->

<div id="loginPage">

    <div class="login-card">

        <div class="login-logo">

            <img
                alt="Dragon Mart Logo"
                crossorigin="anonymous"
            >

        </div>


        <h1>
            Dragon Mart
        </h1>


        <h2>
            Staff Roster Login
        </h2>


        <p class="login-subtitle">
            Please sign in to access the weekly roster
        </p>


        <form id="loginForm">

            <div class="login-field">

                <label for="loginUsername">
                    Username
                </label>

                <input
                    type="text"
                    id="loginUsername"
                    placeholder="Enter username"
                    autocomplete="username"
                    required
                >

            </div>


            <div class="login-field">

                <label for="loginPassword">
                    Password
                </label>

                <div class="password-wrapper">

                    <input
                        type="password"
                        id="loginPassword"
                        placeholder="Enter password"
                        autocomplete="current-password"
                        required
                    >

                    <button
                        type="button"
                        class="show-password"
                        onclick="togglePassword()"
                    >
                        👁️
                    </button>

                </div>

            </div>


            <button
                type="submit"
                class="login-button"
            >
                🔐 Login
            </button>


            <div
                id="loginError"
                class="login-error"
            ></div>

        </form>


        <div class="login-footer">
            Dragon Mart Weekly Staff Roster
        </div>

    </div>

</div>


<!-- =====================================================
     ROSTER AREA
===================================================== -->

<div id="rosterArea">


    <!-- HEADER -->

    <div class="header">

        <div class="logo-container">

            <img
                id="companyLogo"
                src="https://th.bing.com/th/id/OIP.-yQulJpK9XsIT5HcBWQgrAHaHZ?w=108&h=108&c=1&bgcl=d69c3b&am…%22"
                alt="Dragon Mart Logo"
                crossorigin="anonymous"
            >



        </div>


        <h2>
            Dragon Mart Weekly Staff Roster
        </h2>

    </div>


    <!-- WEEK DATE -->

    <div
        id="weekDisplay"
        class="week-display">
    </div>


    <!-- WEEK BUTTONS -->

    <div class="week-controls">

        <button
            class="previous-button"
            onclick="previousWeek()">

            ⬅️ Previous Week

        </button>


        <button
            class="save-week-button"
            onclick="saveCurrentWeek()">

            💾 Save Roster

        </button>


        <button
            class="next-button"
            onclick="nextWeek()">

            Next Week ➡️

        </button>

    </div>


    <!-- TABLE -->

    <table id="rosterTable"></table>

</div>


<!-- =====================================================
     OTHER BUTTONS
===================================================== -->

<div class="controls">

    <button onclick="window.print()">
        🖨️ Print / PDF
    </button>


    <button
        class="csv-button"
        onclick="downloadCSV()">

        ⬇️ Download CSV

    </button>


    <button
        class="image-button"
        onclick="downloadRosterImage()">

        🖼️ Download Roster as Image

    </button>


    <button
        class="add-staff-button"
        onclick="addNewStaff()">

        ➕ Add Staff

    </button>

</div>


<!-- =====================================================
     HTML2CANVAS
===================================================== -->

<script
src="https://cdnjs.cloudflare.com/ajax/libs/html2canvas/1.4.1/html2canvas.min.js">
</script>


<script>


/* =====================================================
   LOGIN DETAILS
===================================================== */

const LOGIN_USERNAME = "Dragon Mart";

const LOGIN_PASSWORD = "CSA2026";


/* =====================================================
   LOGIN CHECK
===================================================== */

function checkLogin() {

    const loggedIn =
        sessionStorage.getItem(
            "DragonMartLoggedIn"
        );


    if (
        loggedIn === "true"
    ) {

        showRoster();

    }

    else {

        showLogin();

    }

}


/* =====================================================
   SHOW LOGIN
===================================================== */

function showLogin() {

    document.getElementById(
        "loginPage"
    ).style.display = "flex";


    document.getElementById(
        "rosterArea"
    ).style.display = "none";


    document.querySelector(
        ".controls"
    ).style.display = "none";

}


/* =====================================================
   SHOW ROSTER
===================================================== */

function showRoster() {

    document.getElementById(
        "loginPage"
    ).style.display = "none";


    document.getElementById(
        "rosterArea"
    ).style.display = "block";


    document.querySelector(
        ".controls"
    ).style.display = "block";

}


/* =====================================================
   LOGIN FORM
===================================================== */

document.getElementById(
    "loginForm"
).addEventListener(
    "submit",
    function(event) {

        event.preventDefault();


        const username =
            document.getElementById(
                "loginUsername"
            ).value.trim();


        const password =
            document.getElementById(
                "loginPassword"
            ).value;


        const error =
            document.getElementById(
                "loginError"
            );


        if (
            username === LOGIN_USERNAME &&
            password === LOGIN_PASSWORD
        ) {

            sessionStorage.setItem(
                "DragonMartLoggedIn",
                "true"
            );


            error.textContent = "";


            showRoster();


            loadCurrentWeek();

        }

        else {

            error.textContent =
                "❌ Incorrect username or password.";

        }

    }
);


/* =====================================================
   SHOW / HIDE PASSWORD
===================================================== */

function togglePassword() {

    const password =
        document.getElementById(
            "loginPassword"
        );


    const button =
        document.querySelector(
            ".show-password"
        );


    if (
        password.type === "password"
    ) {

        password.type = "text";

        button.textContent = "🙈";

    }

    else {

        password.type = "password";

        button.textContent = "👁️";

    }

}


/* =====================================================
   TABLE
===================================================== */

const table =
    document.getElementById(
        "rosterTable"
    );


/* =====================================================
   START DATE
===================================================== */

let startDate =
    new Date(
        2026,
        8,
        7
    );


/* =====================================================
   CURRENT WEEK
===================================================== */

let currentWeek = 0;


/* =====================================================
   DAYS
===================================================== */

const dayNames = [

    "Mon",
    "Tue",
    "Wed",
    "Thu",
    "Fri",
    "Sat",
    "Sun"

];


/* =====================================================
   STAFF LIST
===================================================== */

const staffList = [

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


/* =====================================================
   DESKS
===================================================== */

const desks = [

    "BA",
    "F",
    "H",
    "GA",
    "GD"

];


/* =====================================================
   MANAGEMENT STAFF
===================================================== */

const managementStaff = [

    "Iswary",
    "April"

];


/* =====================================================
   SHIFTS
===================================================== */

const shifts = [

    "AM",
    "PM"

];


/* =====================================================
   STORAGE
===================================================== */

const STORAGE_KEY =
    "DragonMartWeeklyRoster";


/* =====================================================
   USED DESK + SHIFT
===================================================== */

let usedDeskShift =
    Array.from(
        { length: 7 },
        () => new Set()
    );


/* =====================================================
   MID TRACKING
===================================================== */

let midTaken =
    Array.from(
        { length: 7 },
        () => false
    );


/* =====================================================
   WEEK STORAGE KEY
===================================================== */

function getWeekKey() {

    return STORAGE_KEY +
        "_" +
        currentWeek;

}


/* =====================================================
   WEEK START DATE
===================================================== */

function getWeekStartDate() {

    let date =
        new Date(startDate);


    date.setDate(
        startDate.getDate() +
        currentWeek * 7
    );


    return date;

}


/* =====================================================
   FORMAT DATE
===================================================== */

function formatDate(date) {

    return (

        String(
            date.getDate()
        ).padStart(2,"0")

        + "-"

        +

        String(
            date.getMonth() + 1
        ).padStart(2,"0")

        + "-"

        +

        date.getFullYear()

    );

}


/* =====================================================
   UPDATE WEEK DISPLAY
===================================================== */

function updateWeekDisplay() {

    const weekStart =
        getWeekStartDate();


    const weekEnd =
        new Date(weekStart);


    weekEnd.setDate(
        weekStart.getDate() + 6
    );


    document.getElementById(
        "weekDisplay"
    ).innerHTML =

        `Week: ${formatDate(weekStart)}
        &nbsp; - &nbsp;
        ${formatDate(weekEnd)}`;

}


/* =====================================================
   TABLE HEADER
===================================================== */

function createTableHeader() {

    const headerRow =
        table.insertRow(0);


    headerRow.insertCell()
        .outerHTML =
        "<th>Staff Name</th>";


    const weekStart =
        getWeekStartDate();


    for (
        let i = 0;
        i < 7;
        i++
    ) {

        let d =
            new Date(weekStart);


        d.setDate(
            weekStart.getDate() + i
        );


        headerRow.insertCell()
            .innerHTML =

            `<strong>${dayNames[i]}</strong><br>` +

            `<strong>${String(
                d.getDate()
            ).padStart(2,"0")}-` +

            `${String(
                d.getMonth() + 1
            ).padStart(2,"0")}-` +

            `${d.getFullYear()}</strong>`;

    }


    headerRow.insertCell()
        .outerHTML =
        "<th>Remove</th>";

}


/* =====================================================
   DEFAULT SHIFT
===================================================== */

function getDefaultShift(
    day,
    staffName
) {

    if (
        managementStaff.includes(
            staffName
        ) &&
        day <= 4
    ) {

        return "Management-AM";

    }


    return "";

}


/* =====================================================
   SELECT COLOR
===================================================== */

function applySelectColor(s) {

    if (
        s.value === ""
    ) {

        s.className =
            "SelectShift";

    }

    else if (
        s.value.endsWith("-AM") &&
        !s.value.startsWith("Management")
    ) {

        s.className = "AM";

    }

    else if (
        s.value.endsWith("-PM") &&
        !s.value.startsWith("Management")
    ) {

        s.className = "PM";

    }

    else if (
        s.value === "MID"
    ) {

        s.className = "MID";

    }

    else if (
        s.value === "Off"
    ) {

        s.className = "Off";

    }

    else if (
        s.value === "AL"
    ) {

        s.className = "AL";

    }

    else if (
        s.value.startsWith("Management")
    ) {

        s.className = "Management";

    }

}


/* =====================================================
   CREATE SELECT
===================================================== */

function createSelect(
    day,
    staffName,
    savedValue = null
) {

    let s =
        document.createElement("select");


    s.add(
        new Option(
            "Select Shift",
            ""
        )
    );


    let mid =
        new Option(
            "MID",
            "MID"
        );


    if (
        midTaken[day]
    ) {

        mid.disabled = true;

    }


    s.add(mid);


    shifts.forEach(
        sh => {

            desks.forEach(
                d => {

                    let o =
                        new Option(
                            `${d} (${sh})`,
                            `${d}-${sh}`
                        );


                    if (
                        usedDeskShift[day]
                            .has(o.value)
                    ) {

                        o.disabled = true;

                    }


                    s.add(o);

                }
            );

        }
    );


    if (
        managementStaff.includes(
            staffName
        )
    ) {

        shifts.forEach(
            sh => {

                s.add(
                    new Option(
                        `Management (${sh})`,
                        `Management-${sh}`
                    )
                );

            }
        );

    }


    s.add(
        new Option(
            "OFF",
            "Off"
        )
    );


    s.add(
        new Option(
            "AL",
            "AL"
        )
    );


    let valueToUse;


    if (
        savedValue !== null
    ) {

        valueToUse =
            savedValue;

    }

    else {

        valueToUse =
            getDefaultShift(
                day,
                staffName
            );

    }


    s.value =
        valueToUse || "";


    s.oldValue =
        s.value;


    applySelectColor(s);


    if (
        s.value === "MID"
    ) {

        midTaken[day] = true;

    }

    else if (
        s.value &&
        s.value.includes("-") &&
        !s.value.startsWith("Management")
    ) {

        usedDeskShift[day]
            .add(s.value);

    }


    s.onchange =
        function() {

            if (
                s.oldValue === "MID"
            ) {

                midTaken[day] = false;

            }

            else if (
                s.oldValue &&
                s.oldValue.includes("-") &&
                !s.oldValue.startsWith("Management")
            ) {

                usedDeskShift[day]
                    .delete(s.oldValue);

            }


            if (
                s.value === "MID"
            ) {

                midTaken[day] = true;

            }

            else if (
                s.value &&
                s.value.includes("-") &&
                !s.value.startsWith("Management")
            ) {

                usedDeskShift[day]
                    .add(s.value);

            }


            s.oldValue =
                s.value;


            applySelectColor(s);

            update(day);

            updateAllSummaries();

            checkDuplicateDeskShift();

            saveWeekSilently();

        };


    return s;

}


/* =====================================================
   UPDATE OPTIONS
===================================================== */

function update(day) {

    [
        ...table.rows
    ]
    .slice(1)
    .forEach(
        r => {

            if (
                r.classList.contains(
                    "summary-row"
                )
            ) {

                return;

            }


            let cell =
                r.cells[day + 1];


            if (!cell)
                return;


            let s =
                cell.querySelector("select");


            if (!s)
                return;


            [
                ...s.options
            ]
            .forEach(
                o => {

                    if (
                        o.value === "MID"
                    ) {

                        o.disabled =
                            midTaken[day] &&
                            s.value !== "MID";

                    }

                    else if (
                        o.value &&
                        o.value.includes("-") &&
                        !o.value.startsWith("Management")
                    ) {

                        o.disabled =
                            usedDeskShift[day]
                                .has(o.value)
                            &&
                            s.value !== o.value;

                    }

                }
            );

        }
    );

}


/* =====================================================
   ADD ROW
===================================================== */

function addRow(
    name = "",
    savedDays = null
) {

    let r =
        table.insertRow();


    r.insertCell()
        .innerHTML =

        `<input
            value="${name}"
            aria-label="Staff Name"
        >`;


    for (
        let i = 0;
        i < 7;
        i++
    ) {

        let savedValue =
            savedDays
                ? savedDays[i]
                : null;


        r.insertCell()
            .appendChild(
                createSelect(
                    i,
                    name,
                    savedValue
                )
            );

    }


    r.insertCell()
        .innerHTML =

        `<button
            onclick="removeRow(this)">
            ❌
        </button>`;

}


/* =====================================================
   REMOVE ROW
===================================================== */

function removeRow(btn) {

    let r =
        btn.closest("tr");


    if (
        r.classList.contains(
            "summary-row"
        )
    ) {

        return;

    }


    for (
        let i = 0;
        i < 7;
        i++
    ) {

        let s =
            r.cells[i + 1]
                .querySelector("select");


        if (!s)
            continue;


        if (
            s.value === "MID"
        ) {

            midTaken[i] = false;

        }


        if (
            s.value &&
            s.value.includes("-") &&
            !s.value.startsWith("Management")
        ) {

            usedDeskShift[i]
                .delete(s.value);

        }


        update(i);

    }


    r.remove();


    updateAllSummaries();

    checkDuplicateDeskShift();

    saveWeekSilently();

}


/* =====================================================
   DUPLICATE CHECK
===================================================== */

function checkDuplicateDeskShift() {

    [
        ...table.rows
    ]
    .slice(1)
    .forEach(
        r => {

            if (
                r.classList.contains(
                    "summary-row"
                )
            ) {

                return;

            }


            let selections = {};


            [
                ...r.cells
            ]
            .slice(1,8)
            .forEach(
                cell => {

                    let s =
                        cell.querySelector(
                            "select"
                        );


                    if (!s)
                        return;


                    let value =
                        s.value;


                    if (
                        value &&
                        value.includes("-") &&
                        !value.startsWith("Management")
                    ) {

                        if (
                            selections[value]
                        ) {

                            s.classList.add(
                                "duplicate"
                            );

                            s.title =
                                "Duplicate desk + shift!";

                        }

                        else {

                            selections[value] =
                                true;

                            s.classList.remove(
                                "duplicate"
                            );

                            s.title = "";

                        }

                    }

                    else {

                        s.classList.remove(
                            "duplicate"
                        );

                        s.title = "";

                    }

                }
            );

        }
    );

}


/* =====================================================
   SUMMARY
===================================================== */

function createSummaryRow() {

    const oldSummary =
        table.querySelector(
            ".summary-row"
        );


    if (oldSummary) {

        oldSummary.remove();

    }


    const summary =
        table.insertRow();


    summary.className =
        "summary-row";


    summary.insertCell()
        .innerHTML =
        "<strong>Daily Summary</strong>";


    for (
        let day = 0;
        day < 7;
        day++
    ) {

        let cell =
            summary.insertCell();


        cell.id =
            `summary-${day}`;

    }


    summary.insertCell();


    updateAllSummaries();

}


/* =====================================================
   DAILY SUMMARY
===================================================== */

function updateAllSummaries() {

    for (
        let day = 0;
        day < 7;
        day++
    ) {

        const cell =
            document.getElementById(
                `summary-${day}`
            );


        if (!cell)
            continue;


        let counts = {

            AM: 0,
            PM: 0,
            OFF: 0,
            AL: 0,
            MID: 0,
            MANAGEMENT: 0

        };


        [
            ...table.rows
        ]
        .slice(1)
        .forEach(
            row => {

                if (
                    row.classList.contains(
                        "summary-row"
                    )
                ) {

                    return;

                }


                const staffCell =
                    row.cells[day + 1];


                if (!staffCell)
                    return;


                const select =
                    staffCell.querySelector(
                        "select"
                    );


                if (!select)
                    return;


                const value =
                    select.value;


                if (
                    value === "MID"
                ) {

                    counts.MID++;

                }

                else if (
                    value === "Off"
                ) {

                    counts.OFF++;

                }

                else if (
                    value === "AL"
                ) {

                    counts.AL++;

                }

                else if (
                    value.startsWith(
                        "Management"
                    )
                ) {

                    counts.MANAGEMENT++;

                }

                else if (
                    value.endsWith("-AM")
                ) {

                    counts.AM++;

                }

                else if (
                    value.endsWith("-PM")
                ) {

                    counts.PM++;

                }

            }
        );


        cell.innerHTML =

            `<span class="summary-am">
                AM - ${String(counts.AM).padStart(2,"0")}
            </span>
            &nbsp;|&nbsp;

            <span class="summary-pm">
                PM - ${String(counts.PM).padStart(2,"0")}
            </span>
            &nbsp;|&nbsp;

            <span class="summary-off">
                OFF - ${String(counts.OFF).padStart(2,"0")}
            </span>
            &nbsp;|&nbsp;

            <span class="summary-al">
                AL - ${String(counts.AL).padStart(2,"0")}
            </span>
            &nbsp;|&nbsp;

            <span class="summary-mid">
                MID - ${String(counts.MID).padStart(2,"0")}
            </span>

            ${
                counts.MANAGEMENT > 0
                ?
                `&nbsp;|&nbsp;
                <span class="summary-management">
                    MGMT - ${String(
                        counts.MANAGEMENT
                    ).padStart(2,"0")}
                </span>`
                : ""
            }`;

    }

}


/* =====================================================
   SAVE
===================================================== */

function saveCurrentWeek() {

    saveWeekSilently();


    alert(
        "✅ Week saved successfully!"
    );

}


function saveWeekSilently() {

    let rows = [];


    [
        ...table.rows
    ]
    .slice(1)
    .forEach(
        row => {

            if (
                row.classList.contains(
                    "summary-row"
                )
            ) {

                return;

            }


            let input =
                row.cells[0]
                    .querySelector("input");


            let staffName =
                input
                    ? input.value
                    : "";


            let days = [];


            for (
                let day = 0;
                day < 7;
                day++
            ) {

                let select =
                    row.cells[day + 1]
                        .querySelector("select");


                days.push(
                    select
                        ? select.value
                        : ""
                );

            }


            rows.push({

                name:
                    staffName,

                days:
                    days

            });

        }
    );


    localStorage.setItem(
        getWeekKey(),
        JSON.stringify(rows)
    );

}


/* =====================================================
   LOAD CURRENT WEEK
===================================================== */

function loadCurrentWeek() {

    table.innerHTML = "";


    usedDeskShift =
        Array.from(
            { length: 7 },
            () => new Set()
        );


    midTaken =
        Array.from(
            { length: 7 },
            () => false
        );


    createTableHeader();


    let saved =
        localStorage.getItem(
            getWeekKey()
        );


    if (saved) {

        let rows;


        try {

            rows =
                JSON.parse(saved);

        }

        catch {

            rows = [];

        }


        rows.forEach(
            person => {

                addRow(
                    person.name,
                    person.days
                );

            }
        );

    }

    else {

        staffList.forEach(
            name => {

                addRow(name);

            }
        );

    }


    createSummaryRow();


    for (
        let i = 0;
        i < 7;
        i++
    ) {

        update(i);

    }


    checkDuplicateDeskShift();

    updateAllSummaries();

    updateWeekDisplay();

}


/* =====================================================
   ADD NEW STAFF
===================================================== */

function addNewStaff() {

    const name =
        prompt(
            "👤 Enter new staff name:"
        );


    if (
        name === null
    ) {

        return;

    }


    const staffName =
        name.trim();


    if (!staffName) {

        alert(
            "⚠️ Please enter a staff name."
        );

        return;

    }


    let existingNames = [];


    [
        ...table.rows
    ]
    .slice(1)
    .forEach(
        row => {

            if (
                row.classList.contains(
                    "summary-row"
                )
            ) {

                return;

            }


            const input =
                row.cells[0]
                    ?.querySelector("input");


            if (input) {

                existingNames.push(
                    input.value
                        .trim()
                        .toLowerCase()
                );

            }

        }
    );


    if (
        existingNames.includes(
            staffName.toLowerCase()
        )
    ) {

        alert(
            "⚠️ This staff member already exists."
        );

        return;

    }


    const summaryRow =
        table.querySelector(
            ".summary-row"
        );


    if (summaryRow) {

        const row =
            table.insertRow(
                summaryRow.rowIndex
            );


        const nameCell =
            row.insertCell();


        const input =
            document.createElement(
                "input"
            );


        input.value =
            staffName;


        input.setAttribute(
            "aria-label",
            "Staff Name"
        );


        nameCell.appendChild(input);


        for (
            let i = 0;
            i < 7;
            i++
        ) {

            row.insertCell()
                .appendChild(
                    createSelect(
                        i,
                        staffName,
                        ""
                    )
                );

        }


        row.insertCell()
            .innerHTML =

            `<button
                onclick="removeRow(this)">
                ❌
            </button>`;

    }

    else {

        addRow(staffName);

    }


    for (
        let i = 0;
        i < 7;
        i++
    ) {

        update(i);

    }


    updateAllSummaries();

    checkDuplicateDeskShift();

    saveWeekSilently();


    alert(
        `✅ ${staffName} has been added to the roster!`
    );

}


/* =====================================================
   NEXT WEEK
===================================================== */

function nextWeek() {

    saveWeekSilently();

    currentWeek++;

    loadCurrentWeek();

}


/* =====================================================
   PREVIOUS WEEK
===================================================== */

function previousWeek() {

    saveWeekSilently();


    if (
        currentWeek > 0
    ) {

        currentWeek--;

        loadCurrentWeek();

    }

    else {

        alert(
            "This is the first saved week."
        );

    }

}


/* =====================================================
   DOWNLOAD CSV
===================================================== */

function downloadCSV() {

    let csv = [];


    [
        ...table.rows
    ]
    .forEach(
        row => {

            let cols =
                row.querySelectorAll(
                    "th, td"
                );


            let rowData = [];


            cols.forEach(
                (col,index) => {

                    if (
                        index === 0 &&
                        row === table.rows[0]
                    ) {

                        rowData.push(
                            col.innerText.trim()
                        );

                    }

                    else if (
                        index === 0 &&
                        row.classList.contains(
                            "summary-row"
                        )
                    ) {

                        rowData.push(
                            "Daily Summary"
                        );

                    }

                    else if (
                        index === 0
                    ) {

                        let input =
                            col.querySelector(
                                "input"
                            );


                        rowData.push(
                            input
                                ? input.value.trim()
                                : ""
                        );

                    }

                    else if (
                        col.querySelector(
                            "select"
                        )
                    ) {

                        let value =
                            col.querySelector(
                                "select"
                            ).value;


                        rowData.push(

                            value === "Off"
                                ? "OFF"
                                :
                            value ||
                            "Select Shift"

                        );

                    }

                    else {

                        rowData.push(
                            col.innerText
                                .replace(
                                    /\s+/g,
                                    " "
                                )
                                .trim()
                        );

                    }

                }
            );


            csv.push(

                rowData
                    .map(
                        value =>
                            `"${String(value)
                                .replace(
                                    /"/g,
                                    '""'
                                )}"`
                    )
                    .join(",")

            );

        }
    );


    let blob =
        new Blob(
            [csv.join("\n")],
            {
                type: "text/csv"
            }
        );


    let link =
        document.createElement("a");


    link.href =
        URL.createObjectURL(blob);


    link.download =
        "Dragon_Mart_Weekly_Roster.csv";


    document.body.appendChild(link);

    link.click();

    document.body.removeChild(link);

}


/* =====================================================
   DOWNLOAD ROSTER AS IMAGE
===================================================== */

async function downloadRosterImage() {

    const roster =
        document.getElementById(
            "rosterArea"
        );


    if (
        typeof html2canvas ===
        "undefined"
    ) {

        alert(
            "Please wait for the image library to load."
        );

        return;

    }


    const originalSelects =
        roster.querySelectorAll(
            "select"
        );


    const selectedValues =
        Array.from(
            originalSelects
        )
        .map(
            select =>
                select.value
        );


    const clone =
        roster.cloneNode(true);


    clone.style.position =
        "absolute";


    clone.style.left =
        "-100000px";


    clone.style.top =
        "0";


    clone.style.width =
        "1700px";


    clone.style.background =
        "#ffffff";


    clone.style.padding =
        "30px";


    clone.style.boxSizing =
        "border-box";


    const inputs =
        clone.querySelectorAll(
            "input"
        );


    inputs.forEach(
        input => {

            const text =
                document.createElement(
                    "div"
                );


            text.textContent =
                input.value || "";


            text.style.fontFamily =
                '"Segoe UI", Arial, sans-serif';


            text.style.fontSize =
                "17px";


            text.style.fontWeight =
                "700";


            text.style.color =
                "#222222";


            text.style.textAlign =
                "left";


            text.style.padding =
                "8px 12px";


            text.style.width =
                "100%";


            text.style.minWidth =
                "190px";


            text.style.boxSizing =
                "border-box";


            text.style.whiteSpace =
                "nowrap";


            input.parentNode
                .replaceChild(
                    text,
                    input
                );

        }
    );


    const cloneSelects =
        clone.querySelectorAll(
            "select"
        );


    cloneSelects.forEach(
        (
            select,
            index
        ) => {

            const value =
                selectedValues[index] ||
                "";


            let textValue =
                "Select Shift";


            if (
                value === "Off"
            ) {

                textValue = "OFF";

            }

            else if (
                value === "MID"
            ) {

                textValue = "MID";

            }

            else if (
                value === "AL"
            ) {

                textValue = "AL";

            }

            else if (
                value.startsWith(
                    "Management-"
                )
            ) {

                textValue =
                    `Management (${
                        value.replace(
                            "Management-",
                            ""
                        )
                    })`;

            }

            else if (
                value.endsWith("-AM")
            ) {

                textValue =
                    `${value.replace(
                        "-AM",
                        ""
                    )} (AM)`;

            }

            else if (
                value.endsWith("-PM")
            ) {

                textValue =
                    `${value.replace(
                        "-PM",
                        ""
                    )} (PM)`;

            }


            const div =
                document.createElement(
                    "div"
                );


            div.textContent =
                textValue;


            div.style.textAlign =
                "center";


            div.style.fontWeight =
                "700";


            div.style.fontSize =
                "14px";


            div.style.padding =
                "8px 4px";


            div.style.borderRadius =
                "4px";


            div.style.minHeight =
                "34px";


            div.style.display =
                "flex";


            div.style.alignItems =
                "center";


            div.style.justifyContent =
                "center";


            div.style.boxSizing =
                "border-box";


            div.style.width =
                "100%";


            if (
                value.endsWith("-AM") &&
                !value.startsWith("Management-")
            ) {

                div.style.background =
                    "#2196F3";

                div.style.color =
                    "#ffffff";

                div.style.border =
                    "2px solid #1976D2";

            }

            else if (
                value.endsWith("-PM") &&
                !value.startsWith("Management-")
            ) {

                div.style.background =
                    "#4CAF50";

                div.style.color =
                    "#ffffff";

                div.style.border =
                    "2px solid #388E3C";

            }

            else if (
                value === "MID"
            ) {

                div.style.background =
                    "#A0522D";

                div.style.color =
                    "#ffffff";

                div.style.border =
                    "2px solid #7B3F21";

            }

            else if (
                value === "Off"
            ) {

                div.style.background =
                    "#F8D7DA";

                div.style.color =
                    "#721C24";

                div.style.border =
                    "2px solid #E5A1A6";

            }

            else if (
                value === "AL"
            ) {

                div.style.background =
                    "#9C27B0";

                div.style.color =
                    "#ffffff";

                div.style.border =
                    "2px solid #7B1FA2";

            }

            else if (
                value.startsWith(
                    "Management-"
                )
            ) {

                div.style.background =
                    "#FFF3CD";

                div.style.color =
                    "#856404";

                div.style.border =
                    "2px solid #FFDA6A";

            }

            else {

                div.style.background =
                    "#ffffff";

                div.style.color =
                    "#555555";

                div.style.border =
                    "1px solid #cccccc";

            }


            select.parentNode
                .replaceChild(
                    div,
                    select
                );

        }
    );


    const imageTable =
        clone.querySelector(
            "table"
        );


    if (imageTable) {

        imageTable.style.width =
            "100%";


        imageTable.style.tableLayout =
            "fixed";


        imageTable.style.boxShadow =
            "none";


        imageTable.style.borderCollapse =
            "collapse";


        imageTable
            .querySelectorAll("tr")
            .forEach(
                row => {

                    if (
                        row.cells.length > 0
                    ) {

                        row.cells[0]
                            .style.width =
                            "190px";


                        row.cells[0]
                            .style.minWidth =
                            "190px";

                    }


                    if (
                        row.cells.length > 8
                    ) {

                        row.removeChild(
                            row.lastElementChild
                        );

                    }

                }
            );

    }


    clone.querySelectorAll("button")
        .forEach(
            button =>
                button.remove()
        );


    document.body.appendChild(clone);


    try {

        const canvas =
            await html2canvas(
                clone,
                {

                    scale: 2,

                    backgroundColor:
                        "#ffffff",

                    useCORS:
                        true,

                    allowTaint:
                        false,

                    logging:
                        false

                }
            );


        const link =
            document.createElement("a");


        link.download =
            "Dragon_Mart_Weekly_Roster.png";


        link.href =
            canvas.toDataURL(
                "image/png"
            );


        document.body.appendChild(link);

        link.click();

        document.body.removeChild(link);


        alert(
            "✅ Roster image downloaded successfully!"
        );

    }

    catch (error) {

        console.error(error);


        alert(
            "❌ Could not create the roster image."
        );

    }


    if (clone.parentNode) {

        clone.parentNode
            .removeChild(clone);

    }

}


/* =====================================================
   START
===================================================== */

checkLogin();

</script>

</body>

</html>
