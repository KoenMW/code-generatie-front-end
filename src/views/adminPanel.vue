<style>
#card{
    margin: 10px;
    border-radius: 10px;
}
p{
    margin-right: 20px;
}
#title{
    color: #9F82EB;
}
#mainTitle{
    color: #9F82EB;
    margin-top: 20px;
}
hr{
    color: #9F82EB;
}
#functionButton{
    background-color: #9F82EB;
    margin-bottom: 20px;
}
#functionButton:hover{
    background-color: #321A72;
}
</style>

<template>
    <div class="container px-4 py-5" id="hanging-icons">
        <h2 id="title" class="pb-2  ">Admin</h2>
        <hr />
        <div  class="row g-4 py-5 row-cols-1 row-cols-lg-3 ">
            <div id="card" class="col d-flex align-items-start bg-dark">
                <div
                    class="icon-square text-body-emphasis bg-body-secondary d-inline-flex align-items-center justify-content-center fs-4 flex-shrink-0 me-3">
                    <svg class="bi" width="1em" height="1em">
                        <use xlink:href="#toggles2" />
                    </svg>
                </div>
                <div>
                    <h3 id="mainTitle" class="fs-2">All accounts</h3>
                    <p>See all the accounts, add accounts. Also close accounts for users.</p>
                    <RouterLink to="/admin/allAccounts" id="functionButton" class="btn">
                        See accounts
                    </RouterLink>
                </div>
            </div>
            <div id="card" class="col d-flex align-items-start bg-dark">
                <div
                    class="icon-square text-body-emphasis bg-body-secondary d-inline-flex align-items-center justify-content-center fs-4 flex-shrink-0 me-3">
                    <svg class="bi" width="1em" height="1em">
                        <use xlink:href="#tools" />
                    </svg>
                </div>
                <div>
                    <h3 id="mainTitle" class="fs-2">Register accounts</h3>
                    <p>See wich users do not have accounts yet and register accounts</p>
                    <RouterLink to="/admin/NoAccount" id="functionButton" class="btn">
                        Configure accounts
                    </RouterLink>
                </div>
            </div>
            
            <div id="card" class="col d-flex align-items-start bg-dark">
                <div
                    class="icon-square text-body-emphasis bg-body-secondary d-inline-flex align-items-center justify-content-center fs-4 flex-shrink-0 me-3">
                    <svg class="bi" width="1em" height="1em">
                        <use xlink:href="#tools" />
                    </svg>
                </div>
                <div>
                    <h3 id="mainTitle" class="fs-2">Configure accounts</h3>
                    <p>Change account limits</p><br>
                    <RouterLink to="/configureLimit" id="functionButton" class="btn ">
                        Configure accounts
                    </RouterLink>
                </div>
            </div>
            <div id="card" class="col d-flex align-items-start bg-dark">
                <div
                    class="icon-square text-body-emphasis bg-body-secondary d-inline-flex align-items-center justify-content-center fs-4 flex-shrink-0 me-3">
                    <svg class="bi" width="1em" height="1em">
                        <use xlink:href="#cpu-fill" />
                    </svg>
                </div>
                <div>
                    <h3 id="mainTitle" class="fs-2">Transactions</h3>
                    <p>Perform transactions for accounts</p><br>
                    <RouterLink to="/admin/transaction" id="functionButton" class="btn ">
                        Make transactions
                    </RouterLink>
                </div>
            </div>
            <div id="card" class="col d-flex align-items-start bg-dark">
                <div
                    class="icon-square text-body-emphasis bg-body-secondary d-inline-flex align-items-center justify-content-center fs-4 flex-shrink-0 me-3">
                    <svg class="bi" width="1em" height="1em">
                        <use xlink:href="#cpu-fill" />
                    </svg>
                </div>
                <div>
                    <h3 id="mainTitle" class="fs-2">NovaBank account</h3>
                    <p>See the NovaBank account</p><br>
                    <RouterLink to="/admin/bankOwnAccount" id="functionButton" class="btn ">
                        See account
                    </RouterLink>
                </div>
            </div>

            <div id="card" class="col d-flex align-items-start bg-dark">
                <div
                    class="icon-square text-body-emphasis bg-body-secondary d-inline-flex align-items-center justify-content-center fs-4 flex-shrink-0 me-3">
                    <svg class="bi" width="1em" height="1em">
                        <use xlink:href="#cpu-fill" />
                    </svg>
                </div>
                <div>
                    <h3 id="mainTitle" class="fs-2">User management</h3>
                    <p>Change day and transaction limit for users, and add users</p><br>
                    <RouterLink to="/userOverview" id="functionButton" class="btn ">
                        See users
                    </RouterLink>
                </div>
            </div>
            
        </div>
    </div>
</template>
  
<script>
import { RouterLink } from 'vue-router';

export default {
    data() {
        return {};
    },
    methods: {},
    components: { RouterLink }
}
</script>