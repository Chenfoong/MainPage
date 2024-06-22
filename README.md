/* Basic styling for body and main content */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
}

main {
    flex: 1;
    padding: 20px;
}

/* Sidebar container */
.sidebar {
    height: 100vh;
    width: 250px;
    position: fixed;
    top: 0;
    left: 0;
    background-color: #333;
    color: white;
    padding-top: 20px;
    transition: width 0.3s;
}

/* Sidebar header */
.sidebar .header {
    padding: 15px;
    text-align: center;
    font-size: 20px;
    font-weight: bold;
    background-color: #444;
}

/* Sidebar links */
.sidebar a {
    padding: 10px 15px;
    text-decoration: none;
    font-size: 18px;
    color: white;
    display: block;
    transition: background-color 0.3s;
}

.sidebar a:hover {
    background-color: #575757;
}

/* Toggle button for sidebar */
.toggle-btn {
    position: absolute;
    top: 15px;
    left: 250px;
    font-size: 20px;
    background-color: #333;
    color: white;
    border: none;
    cursor: pointer;
    transition: left 0.3s;
}

.toggle-btn.collapsed {
    left: 0;
}

/* Collapsed sidebar */
.sidebar.collapsed {
    width: 60px;
}

.sidebar.collapsed .header {
    display: none;
}

.sidebar.collapsed a {
    text-align: center;
    padding: 10px;
}

.sidebar.collapsed a span {
    display: none;
}

.sidebar.collapsed a::before {
    content: attr(data-icon);
    font-size: 18px;
}
