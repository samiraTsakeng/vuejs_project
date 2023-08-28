<template>
    <nav class="navbar">
        <h2 class="navbar-logo"><a href="#">Internship App</a></h2>
        <div class="navbar-menu ">
             <a href="index.html">Home</a>
            <a href="#about">About</a> 
            <a href="#Services">Services</a>
            <!--<a href="#index.html">Home</a>-->
            <a href="#company">Companies</a>
            <div class="dropdown">
                <button class="dropbtn">Register</button>
                <div class="dropdown-content">
                  <a href="intern form.html">Intern</a>
                  <a href="job_seeker_form.html">Job seeker</a>
                  <a href="Company form.html">Company</a>
                </div>
              </div>
           
        </div>
        <div class="Menu-toggle">
            <span class="bar"></span>
            <span class="bar"></span>
            <span class="bar"></span>
        </div>
    </nav>
</template>

<script>
export default {
    name: 'NavComponent'
}
</script>
