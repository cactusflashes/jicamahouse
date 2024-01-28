<style>
    .nav-wrapper {
        background-color: rgba(12, 59, 46, .5);
        -webkit-backdrop-filter: blur(10px);
        backdrop-filter: blur(10px);    
        height: 60px;
        width: 100%; 
        display: flex;
        align-items: center;
        justify-content: flex-end;
        flex-direction: row;
        position: fixed; 
        z-index: 10;
        border-bottom: 1px solid rgba(255, 255, 255, .2);  
    }
    
    ul {
        list-style: none;
        display: flex;
        flex-direction: row;
        padding-right: 80px;
        gap: 5%; 
    }
    
    li {
        display: flex;
        font-family: 'Inter', sans-serif;
        font-weight: 500;
        font-size: 1rem;
        padding: 10px 10px;
        border-radius: 16px;
        transition: background-color 0.5s, color 0.5s, border 0.3s;
        border: 1px solid transparent;
    
    }
    
    li:hover {
        display: flex;
        font-family: 'Inter', sans-serif;
        cursor: pointer;
        transition: background-color 0.5s, color 0.5s, border 0.3s;
    }
    
    a {
        transition: background-color 0.5s, color 0.5s, border 0.3s;
        text-decoration: none;
        color: #ecefee; 
        transition: text-decoration .2s, color .2s; 

    }
    
    li:hover a {
        transition: color 0.2s; 
        text-decoration: underline;
        color: #dce48b; 
        transition: text-decoration .2s, color .2s; 
    }

    
    @media all and (max-width: 700px) {
        .nav-wrapper {
            align-items: center;
            justify-content: center;
        }
    
        ul {
            gap: 5%;  
            justify-content: center;
            padding: 0;
            margin: 0; 
        }
    
        li {
            font-weight: 600;
            font-size: 1rem;
        }
    }
    
    </style>
    
    <script>
    </script>
    
    
    <div class="nav-wrapper">
        <ul>
            <li><a href="/">Home</a></li>
            <li><a href="/about">About</a></li>
            <li><a href="/contact">Contact</a></li>
        </ul>
    </div>