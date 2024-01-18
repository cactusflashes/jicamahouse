<style>
    .footer-bar {
        display: flex; 
        flex-direction: column;
        height: 180px; 
        width: 100%;
        background-color: #0c3b2e;
        align-items: center;
        justify-content: center;
        color: #ecefee; 
        position: relative;
    }

    .footer-bar::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    right: 0;
    bottom: 0;
    background: rgba(0, 0, 0, 0.4); /* Adjust the opacity as needed */
    z-index: 2;
}


    .col-vert {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center; 
        gap: 50%;
        z-index: 3;
    }

    a {
        font-family: 'Inter', sans-serif;
        font-size: 1rem; 
        font-weight: 400;
        color: #ecefee; 
    }
</style>

<div class="footer-bar">
        <div class="col-vert">
            <h2>©2024 Jicamahouse Photo</h2>
                <div class="text-spacer"></div>
            <h2 style="opacity: 60%;">tessandra.studio@gmail.com</h2>
                <div class="text-spacer"></div>
                <div class="text-spacer"></div>
            <a href="/instagram" style="opacity: 60%;">Find me on Instagram ›</a>
        </div>
</div>