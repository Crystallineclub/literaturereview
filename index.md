---
layout: default
---

<div class="container">
    <h1>Crystalline Rock Chemistry (CrysChem) Database</h1>
    <p>The Crystalline Rock Chemistry (CrysChem) database, presented by the Crystalline Rock Club (CRC), is a comprehensive BibTeX reference file containing hydrogeochemical data and chemical process models relevant to nuclear waste repositories in crystalline rock. Designed for use with reference manager software, the database includes abstracts, tags for specific data, and excludes full papers, aiming to facilitate the organized and accessible exchange of information crucial for deep geologic repository science.</p>

    <!-- Tab buttons -->
    <div>
        <button class="tab-button" onclick="openTab(event, 'About')">About</button>
        <button class="tab-button" onclick="openTab(event, 'Report')">Report</button>
        <button class="tab-button" onclick="openTab(event, 'Database')">Database</button>
        <button class="tab-button" onclick="openTab(event, 'Contact')">Contact Us</button>
    </div>

    <!-- Tab content -->
    <div id="About" class="tab-content">
        <h2>About</h2>
        <p>Details about the CrysChem database and its purpose.</p>
        <a href="./another-page.html">Learn more</a>
    </div>

    <div id="Report" class="tab-content">
        <h2>Report</h2>
        <p>Information regarding reports related to the CrysChem database.</p>
        <a href="./report.html">View Report</a>
    </div>

    <div id="Database" class="tab-content">
        <h2>Database</h2>
        <p>Access the hydrogeochemical data and chemical process models.</p>
        <a href="./database.html">Explore Database</a>
    </div>

    <div id="Contact" class="tab-content">
        <h2>Contact Us</h2>
        <p>Get in touch for more information or inquiries.</p>
        <a href="./contactus.html">Contact Information</a>
    </div>
</div>

<style>
    .container {
        text-align: center;
        margin: 20px;
    }
    .tab-content {
        display: none; /* Hide all tab content by default */
        margin-top: 20px;
    }
    .tab-button {
        padding: 10px 20px;
        cursor: pointer;
        background-color: #f1f1f1;
        border: none;
        border-bottom: 2px solid transparent;
        transition: background-color 0.3s;
        margin: 5px;
    }
    .tab-button:hover {
        background-color: #ddd;
    }
    .active {
        background-color: #fff;
        border-bottom: 2px solid #007bff; /* Active tab color */
    }
</style>

<script>
    // Function to open a tab
    function openTab(evt, tabName) {
        // Hide all tab content
        var i, tabcontent, tabbuttons;
        tabcontent = document.getElementsByClassName("tab-content");
        for (i = 0; i < tabcontent.length; i++) {
            tabcontent[i].style.display = "none";
        }

        // Remove the active class from all buttons
        tabbuttons = document.getElementsByClassName("tab-button");
        for (i = 0; i < tabbuttons.length; i++) {
            tabbuttons[i].className = tabbuttons[i].className.replace(" active", "");
        }

        // Show the current tab and add an "active" class to the button that opened the tab
        document.getElementById(tabName).style.display = "block";
        evt.currentTarget.className += " active";
    }

    // Open the first tab by default
    document.addEventListener("DOMContentLoaded", function() {
        document.querySelector(".tab-button").click();
    });
</script>
