<template>
    <div class="hello">
        <div class="header">
            <div class="menu-icon">
                <div class="container">
                    <div></div>
                    <div></div>
                    <div></div>
                </div>
            </div>
            <div class="logo">
                <img src="../assets/img/logo.svg" alt="patricia logo">
            </div>
            <div class="actions">
                <div><img src="../assets/img/notification.svg" alt="notification"></div>
                <div><img src="../assets/img/mail.svg" alt="message"></div>
                <div><img src="" alt="profile"></div>
            </div>
        </div>

        <div class="body">
            <div class="nav">
                <ul>
                    <li>
                        <img src="../assets/img/menu.png" alt="menu icon">
                        <span>Overview</span>
                    </li>
                    <li>
                        <img src="../assets/img/buy.png" alt="transactions icon">
                        <span>Transactions</span>
                    </li>
                    <li>
                        <img src="../assets/img/wallet.png" alt="wallet icon">
                        <span>Wallet</span>
                    </li>
                    <li>
                        <img src="../assets/img/gift.png" alt="products icon">
                        <span>Products</span>
                    </li>
                    <li>
                        <img src="../assets/img/graph.png" alt="rates icon">
                        <span>Rates</span>
                    </li>
                    <li>
                        <img src="../assets/img/settings.png" alt="suggestions icon">
                        <span>Suggestions</span>
                    </li>
                    <li>
                        <img src="../assets/img/settings.png" alt="settings">
                        <span>Settings</span>
                    </li>
                </ul>
            </div>
            <div class="sub-nav">
                <ul>
                    <li>
                        <span>Messages</span>
                        <button>New Message</button>
                    </li>
                    <li>
                        <div>
                            <span>Deposit Issue</span>
                            <span class="small">4</span>
                        </div>
                        <p>3 minutes ago <img src="../assets/img/attachment.svg" alt="attachment"></p>
                    </li>
                    <li>
                        <div>
                            <span>Deposit Issue</span>
                            <span class="small">4</span>
                            <img class="delete-btn" src="../assets/img/delete.svg" alt="delete" />
                        </div>
                        <p>3 minutes ago <img src="../assets/img/attachment.svg" alt="attachment"></p>
                    </li>
                    <li>
                        <div>
                            <span>Deposit Issue</span>
                            <span class="small">4</span>
                        </div>
                        <p>3 minutes ago <img src="../assets/img/attachment.svg" alt="attachment"></p>
                    </li>
                    <li>
                        <div>
                            <span>Deposit Issue</span>
                            <span class="small">4</span>
                        </div>
                        <p>3 minutes ago <img src="../assets/img/attachment.svg" alt="attachment"></p>
                    </li>
                    <li>
                        <div>
                            <span>Deposit Issue</span>
                            <span class="small">4</span>
                        </div>
                        <p>3 minutes ago <img src="../assets/img/attachment.svg" alt="attachment"></p>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',

  data () {
    return {}
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    ul, li {
        list-style: none;
        padding: 0;
        margin: 0;
    }

    .menu-icon .container {
        display: flex;
        align-items: baseline;
    }

    .menu-icon .container div {
        width: 4px;
        height: 30px;
        background: #000;
        margin-left: 7px;
    }
    .menu-icon .container div:last-child {
        height: 20px;
    }

    .menu-icon, .logo, .actions {
        display: flex;
    }

    .header {
        display: flex;
        padding: 30px 0;
    }

    .menu-icon {
        width: 14%;
        justify-content: center;
    }

    .logo {
        width: 20%;
        padding-left: 30px;
    }

    .actions {
        width: calc(100% - 34%);
        justify-content: flex-end;
    }

    .actions div {
        width: 10%;
        text-align: center;
    }

    .actions img {
        width: 30%;
    }

    .body {
        display: flex;
        height: calc(100vh - 92.5px);
    }

    .nav {
        width: 14%;
    }

    .nav  li img {
        width: 15%;
    }

    .nav  li {
        display: flex;
        align-items: center;
        margin: 60px 0 60px 20px;
        color: #928f8f;
    }

    .nav ul {
        margin-left: 20px;
    }

    .nav  li:first-child {
        box-shadow: 1px 1px 10px 5px #eee;
        padding: 10px 20px;
        margin: 40px 20px;
    }

    .nav  li span {
        padding-left: 20px;
    }

    .sub-nav {
        background: #f4f5f9;
        width: 20%;
    }

    .sub-nav li {
        border-bottom: 1px solid #ebecec;
        padding: 25px 80px 25px 20px;
        color: #373738;
    }

    .sub-nav li:first-child {
        padding: 55px 0 55px 20px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .sub-nav li:nth-child(3) {
        background: #fff;
        border-left: 2px solid #2c9cdb;
    }

    .sub-nav li:first-child button {
        margin-right: 15px;
        padding: 10px 15px;
        border-radius: 20px;
        border: none;
        background: #2c9cdb;
        color: white;
    }

    .sub-nav li div > span {
        font-weight: bold;
    }

    .sub-nav div img {
        color: red;
        width: 7%;
    }

    .sub-nav li:not(:first-child) > p {
        color: #cfcfcf;
        margin-top: 10px;
        margin-bottom: 0;
        font-size: .8rem;
    }

    .sub-nav p img {
        width: 5%;
        padding-left: 10px;
    }

    .sub-nav li div {
        display: flex;
        justify-content: space-between;
        align-items: center;
        position: relative;
    }

    .sub-nav li .small {
        padding: 5px 20px;
        background: rgba(44, 156, 219, .3);
        color: #2c9cdb;
        border-radius: 20px;
        font-size: .7rem;
        font-weight: lighter;
    }

    .sub-nav li .delete-btn {
        position: absolute;
        right: -50px;
    }
</style>
