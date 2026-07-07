# Advanced-CS33
/* CSS Variables */
:root{
    --bg:#ffffff;
    --text:#222;
    --primary:#0077cc;
}

body{
    margin:0;
    font-family:Arial,sans-serif;
    background:var(--bg);
    color:var(--text);
}

/* Header */
header{
    background:var(--primary);
    color:white;
    padding:20px;
    text-align:center;
}

/* Navigation using Flexbox */
nav ul{
    display:flex;
    justify-content:center;
    gap:20px;
    list-style:none;
    padding:0;
    margin:0;
    flex-wrap:wrap;
}

nav a{
    color:white;
    text-decoration:none;
}

/* Main layout using CSS Grid */
.container{
    display:grid;
    grid-template-columns:1fr;
    gap:20px;
    padding:20px;
}

/* Project Cards */
.projects{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
    gap:20px;
}

.card{
    background:#f4f4f4;
    padding:20px;
    border-radius:10px;
    box-shadow:0 2px 8px rgba(0,0,0,0.1);
}

/* Responsive Images */
img{
    max-width:100%;
    height:auto;
    display:block;
}

/* Tablet */
@media (min-width:768px){
    .container{
        grid-template-columns:1fr 2fr;
    }
}

/* Desktop */
@media (min-width:1024px){
    .container{
        grid-template-columns:1fr 3fr;
    }
}

/* Dark Theme */
.dark-theme{
    --bg:#121212;
    --text:#ffffff;
    --primary:#4dabf7;
}
