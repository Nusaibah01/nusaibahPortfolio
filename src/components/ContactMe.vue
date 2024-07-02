<template>
    <div class="container-fluid" id="contactUs">
       <h2>Get in touch with Me:</h2>
        
        
        <form action="https://formspree.io/f/xpzvvlqj" method="post">
      <input type="text" placeholder="First Name" name="First Name"  class="i" required><br>
      <input type="text" placeholder="Last Name" name="Last Name" class="i" required><br>
      <input type="email" placeholder="Email Address" name="Email Address" class="i" required><br>
      <textarea rows="5" cols="60" placeholder="Your message" name="Your message" required></textarea><br>
      <button type="submit" id="b">Submit</button>
    </form>
    
   

    </div>
</template>

<script>
</script>
<style scoped>
 h2{
    color: #0C0C0C;
    font-family: "Press Start 2P", system-ui;
 }
 input, textarea{
    color: blue;
    font-family: "Space Mono", monospace;
    background-color: #0C0C0C;
 }
 input{
    border: white;
    width: 610px ;
    padding: 30px;
    margin: 30px;
 }

#reachMe{
    background-color: black;
}
button{
    border-radius: 5px;
    background-color: antiquewhite;
    margin: 30px;
}
</style>
