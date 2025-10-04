<style>
/* https://www.dafont.com/cynatar.font */
@font-face {
    font-family: 'Cynatar';
    src: url('Cynatar.otf') format('opentype');
    font-weight: normal;
    font-style: normal;
    font-display: swap;
}

body {
    font-family: 'Berkeley Mono', monospace;
    background-color: #000000;
    color: #FFD400;
    margin: 0;
    min-height: 100vh;
    /* Use flex column so footer can be pushed to the bottom when content is short */
    display: flex;
    flex-direction: column;
}

header {
    display: flex;
    align-items: flex-start;
    /* align to left side of the header column */
    justify-content: flex-start;
    flex-direction: column;
    /* stack the three titles */
    gap: 0.75rem;
    /* push header content roughly 1/3 from the left edge of the viewport */
    padding: 2rem 1rem 2rem 33.333vw;
}

/* Ensure the header title keeps the Cynatar pink color whether the
   markup is <h1><a> or <a><h1>. */
header h1,
header h1 a,
header a h1,
header>a h1 {
    /* two-tone misprint: yellow front, pink offset behind */
    color: #FFD400;
    /* front (visible) color */
    font-family: 'Cynatar', sans-serif;
    font-size: 3.5rem;
    line-height: 1;
    /* pink sharp offset first, then pink glows and dark base shadow */
    text-shadow:
        -4px 2px 0 #FF2D95,
        /* pink misprint offset behind */
        0 0 12px rgba(255, 45, 149, 0.95),
        0 0 32px rgba(255, 45, 149, 0.65),
        0 8px 40px rgba(0, 0, 0, 0.85);
    margin: 0;
}
</style>

<body>
    <header>
        <a href="https://ramblings.0x53a.com">
            <h1>0x53A</h1>
        </a>
    </header>
</body>
