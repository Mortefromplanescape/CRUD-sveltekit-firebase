<script>
    let email = "";
    let password = "";
    let confirmPass = "";
</script>

<div class="authContainer">
    <form>
        <h1>Login</h1>
        <label>
            <p class={email ? 'above' : 'center'}>E-mail</p>
            <input bind:value={email} type="email" placeholder="E-mail" />
        </label>
        <label>
            <p class={password ? 'above' : 'center'}>Password</p>
            <input bind:value={password} type="password" placeholder="Password" />
        </label>
        <label>
            <p class={confirmPass ? 'above' : 'center'}>Confirm Password</p>
            <input bind:value={confirmPass} type="password" placeholder="Confirm Password" />
        </label>
        <button type="button">Submit</button>
    </form>
</div>

<style>
    .authContainer {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        flex: 1;
        padding: 24px;
    }

    form {
        display: flex;
        flex-direction: column;
        gap: 14px;
        width: 400px;
        max-width: 100%;
        margin: 0 auto;
    }

    form label {
        position: relative;
        border: 1px solid darkolivegreen;
        border-radius: 5px;
    }

    form input {
        width: 100%;
        border: none;
        background: transparent;
        color: white;
        padding: 14px;
    }

    form input:focus {
        border: none;
        outline: none;
    }

    form button {
        background: darkolivegreen;
        color: white;
        border: none;
        padding: 14px 0;
        border-radius: 5px;
        cursor: pointer;
        font-size: 1.2rem;
    }

    form button:hover {
        background: green;
    }

    h1 {
        text-align: center;
        font-size: 3rem;
    }

    .above,
    .center {
        position: absolute;
        transform: translateY(-50%);
        pointer-events: none;
        color: white;
        border-radius: 4px;
        padding: 0 6px;
        font-size: 0.8rem;
    }
</style>