<template>
  <div class="about">
    <header class='masthead'>
      <p class='masthead-intro'> Hello we're </p>
      <h1 class='masthead-heading'> CBGA Ethiopia!</h1>
    </header>
    <section class="introduction-section">
      <h1> Who are we? </h1>
      <p> We are students from Beaumont High, soon to be web developers. We love the internet and technology. We feel that
        we can do something from technology as a job in the future if we strive to achieve our wants. </p>
    </section>
    <section class="location-section">
      <h1> Where are we from? </h1>
      <p>
        <b> Hailemelekot: </b> Although I was born in Injibara, I currently live and was raised in bahirdar. <br> <br>
        <b> Hailemelekot: </b> Although I was born in Injibara, I currently live and was raised in bahirdar. <br><br>
      </p>
    </section>
    <section class="questions-section">
      <h1> More About Us </h1>
      <h2> What are our favorite hobbies?</h2>
      <p> One of our favorite hobbies are sports. Although we might play different sports, we have a strong passion for
        the sport that we do. Another big hobby we have is coding. We like giving ourselves challenges and coding is a big
        one.</p>
      <h2> What's our dream jobs? </h2>
      <p> One of our dream jobs that we are trying to achieve currently are becoming web developers. </p>
      <h2> Why do we want to be web developers? </h2>
      <p> Coding and programming are awesome because the internet is built on these two features. We want to be web
        developers because we wish to get a job in the future that surrounds the work of coding and programming. </p>
    </section>
  </div>
</template>


<style scoped>
.about {
  color: #222222;
  font-size: 1em;
  font-family: Cambria, Cochin, Georgia, Times, 'Times New Roman', serif;
}

.masthead-heading,
.masthead-intro {
  text-align: center;
}

.masthead {
  padding: 6em 0;
  background-size: cover;
  background-repeat: no-repeat;
}

.masthead-intro {
  margin-bottom: 0.1em;
  font-size: 2em;
  color: rgb(171, 160, 255);
  font-weight: bold;
}

.masthead-heading {
  color: #ffffffcf;
  margin-top: -0.2em;
  font-family: "Open Sans", "Helvetica Neue", sans-serif;
  font-weight: bold;
  font-size: 6em;
  letter-spacing: -0.02em;
  text-transform: uppercase;
}

.introduction-section,
.location-section,
.questions-section {
  max-width: 38em;
  margin-left: auto;
  margin-right: auto;
  margin-top: 2em;
}

.introduction-section>p,
.location-section>p,
.questions-section {
  font-weight: 300;
  letter-spacing: 0.01em;
}

.questions-section>h2 {
  font-family: "Gentium Book Basic", Georgia, serif;
  font-size: 1.2em;
  font-weight: bold;
  margin: 2em 0 1em 0;
}

section>h1 {
  margin-top: 2em;
}

.masthead-heading,
.masthead-intro {
  text-align: center;
}

.masthead {
  padding: 6em 0;
  background-image: url('@/assets/writing\ mat.jpg');
  background-size: cover;
  background-repeat: no-repeat;
}

.masthead-intro {
  margin-bottom: 0.1em;
  font-family: "Gentium Book Basic", Georgia, serif;
  font-size: 2em;
}

.masthead-heading {
  margin-top: -0.2em;
  font-family: "Open Sans", "Helvetica Neue", sans-serif;
  font-weight: bold;
  font-size: 5em;
  text-transform: uppercase;
}

.introduction>p,
.location>p {
  font-weight: 300;
}

h2 {
  font-family: "Gentium Book Basic", Georgia, serif;
  font-size: 1.2em;
  font-weight: bold;
}

.introduction-section,
.location-section,
.questions-section {
  max-width: 38em;
  margin-left: auto;
  margin-right: auto;
  margin-top: 2em;
}

@media only screen and (max-width: 500px) {
  .masthead {
    padding: 3em 0;
  }

  .masthead-heading {
    font-size: 3em;
  }
}
</style>