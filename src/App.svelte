<script lang="ts">
    import Logo from '/belkot.svg';
</script>

<main>
    <img id="logo" src={Logo} alt="Logo"/>

    <form>
        <h1> Belkot </h1>
        <label> Username <input type="text" name="username"></label>  
        <label> Password <input type="password" name="password"></label>
        <button type="submit"> Log in </button>
    </form>

    <button id="signup"> Sign up </button>
</main>

<style lang="scss">
    main {
        width: 100%;
        height: 100%;
        background-color: #040404;
        font-family: 'Courier New', 'monospace';
        
        flex-direction: column;
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 20px;
    }  
    
    h1 {
        font-weight: normal;
        padding: 0;
        text-align: center;
        margin: 0;
        margin-top: 15px;
    }

    #logo { height: 100px }
    
    form {
        font-size: 24px;
        border: 1px solid white;
        border-radius: 10px;
        padding: 10px;
        color: white;
        width: 400px;
        display: flex;
        flex-direction: column;
        
        label {
            margin-top: 30px;
            text-align: center;
            display: flex;
            flex-direction: column;
            gap: 4px;

            input {
                font-size: 24px;
                color: white;
                background: none;
                border: unset;
                text-align: center;
                border-bottom: 1px solid white;
                border-radius: 5px;
            }
        } 

        button {
            margin-top: 10px;
            border: unset;
            border-radius: 5px;
            height: 40px;
            font-size: 24px;
            font-family: 'Courier New', 'monospace';
            letter-spacing: -1px;
        }
    }

    #signup:hover { text-decoration: underline }

    #signup {
        background: none;
        border: unset;
        color: white;
        font-size: 24px;
    }
</style>
