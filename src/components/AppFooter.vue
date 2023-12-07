<template>
  <div class="footer">
    <div class="footerLeft">
      <div class="footerLeftHeader">CBGA</div>
      <div class="footerLeftLabel">
        CBGA is a Non-governmental Organization established in Ethiopia in order to
        advocate for robust budgetary governance throughout government organizations and
        goal orientation towards Sustainable Development Goals
      </div>
    </div>
    <div class="footerRightLeftContainer">
      <div class="footerRight">
        <div class="footerRightHeader">Company</div>
        <div class="footerRightLabel">About</div>
        <div class="footerRightLabel">Blogs</div>
        <div class="footerRightLabel">Jobs</div>
        <div class="footerRightLabel">Press</div>
        <div class="footerRightLabel">Partners</div>
      </div>
      <div class="footerRight">
        <div class="footerRightHeader">Legal</div>
        <a class="footerRightLabel" href="http://localhost:8080/privacy"
          >Terms and Policies</a
        >
        <div class="footerRightLabel">Claims</div>
        <div class="footerRightLabel">Conditions</div>
        <div class="footerRightLabel">Help</div>
      </div>
    </div>
    <div class="footerRight">
      <div class="footerRightHeaderS">SUBSCRIBE</div>
      <div class="footerRightLabelLatest">
        The latest news, articles, and resources, sent to your inbox weekly.
      </div>
      <input class="email" type="email" placeholder="Enter Email" />
      <input class="subscribe" type="button" value="Subscribe" />
    </div>
  </div>
</template>
<script>
export default {};
</script>

<style scoped>
.footer {
  background-color: rgb(15 23 42);
  color: rgb(208, 208, 208);
  padding: 10px 50px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: flex-start;
  gap: 10px;
  font-family: sans-serif;
}
.footerRightLeftContainer {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  width: fit-content;
  flex: 2;
  width: 100%;
}
.footerLeft {
  display: flex;
  flex-direction: column;
  gap: 6px;
  padding: 10px;
  flex: 3;
}
.footerLeftHeader {
  font-size: 16px;
  font-weight: bold;
}
.footerLeftLabel {
  font-size: 15px;
  padding: 10px 0px;
  line-height: 1.7rem;
}

.footerRight {
  display: flex;
  flex-direction: column;
  gap: 6px;
  flex: 2;
  padding: 10px;
}
.footerRightHeader {
  font-size: 16px;
  font-weight: bold;
}
.footerRightHeaderS {
  font-size: 16px;
  font-weight: bold;
  text-align: center;
}
.footerRightLabel {
  font-size: 15px;
  font-weight: 600;
  padding: 5px 0px;
  color: rgba(181, 255, 239, 0.666);
  cursor: pointer;
}
.footerRightLabel:hover {
  color: rgba(145, 149, 255, 0.666);
}
.footerRightLabelLatest {
  font-size: 14px;
  text-align: justify;
}
.email {
  font-size: 15px;
  padding: 8px;
  margin: 5px;
  outline: none;
  border-radius: 4px;
  border: none;
  text-align: center;
}
.subscribe {
  font-size: 15px;
  padding: 10px;
  font-weight: bold;
  margin: 5px;
  outline: none;
  background-color: rgb(66, 193, 151);
  cursor: pointer;
  border-radius: 30px;
  border: none;
  transition: all 0.5s ease-in-out;
}
.subscribe:hover {
  background-color: rgb(111, 255, 207);
}

@media screen and (max-width: 900px) {
  .footerLeftLabel {
    font-size: 14px;
  }
}
@media screen and (max-width: 880px) {
  .footer {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 5px;
  }
  .footerRightLabel {
    font-size: 11px;
  }
  .footerRightHeader {
    font-size: 14px;
  }
}
</style>
