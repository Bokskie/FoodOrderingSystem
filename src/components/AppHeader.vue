<template>
    <header>
        <div class="nav-bar">
            <div class="sidebar-button">
                <button @click="show"><span class="material-symbols-sharp">menu</span></button>
            </div>
            <div class="dashboard">
                <h1>DashBoard</h1>
            </div>
            <div class="search-box">
                <form action="" method="">
                    <input type="search" placeholder="Search...">
                    <button>
                        <span class="material-symbols-sharp">search</span>
                    </button>
                </form>    
            </div>
            <div class="user-profile">
                <span class="material-symbols-sharp">person</span>
            </div>
        </div>
    </header>
   
</template>

<script>
   export default {
       methods: {
           show(){
               this.$emit("buttonCliked")
           }
       }
   }

</script>

<style scoped>

header 
{
    background: #464646
}
header button
{
    cursor: pointer;
}
header .nav-bar 
{
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-between;
}
header .sidebar-button button 
{
    background: #00aa6c;
    border-radius: 3rem;
    position: relative;
    left: 1rem;
    top: 1.5rem;
    width: 4rem;
    height: 3rem;
}
header .nav-bar .search-box
{
    background: #ffffff;
    border-radius: 3rem;
    position: relative;
    top: 0.5rem;
    padding: 10px;
    height: 3rem;
}
header .nav-bar .search-box input 
{
    border: none;
    outline: none;
    border-radius: 3rem;
    padding: 10px;
    position: relative;
    bottom: 0.2rem;
}
header .nav-bar .search-box button 
{
    border: none;
    border-radius: 3rem;
    padding: 10px;
    background: #00aa6c;
}
</style>