<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <p>
      Fulminology Labs provides an engineering arm for small and growing businesses. We build software that<br>
      alleviates friction in your day-to-day operations that arise from the use of isolated platforms or manual data entry.<br>
      <a>Reach out to nick@fulminolgylabs.co for inquiries.</a>
    </p>

    <hr>

    <h2>Highlighted Cases</h2>
    <div class="highlights"> 
      <div class="card">
        <h4>Automated Client Onboarding</h4>
        <hr>
          <p>It takes a lot for financial advisors to dilligence their clients and often times all they get is a
          large manilla folder with investment statements and tax returns. We've used Plaid, a popular product embedded in many
          applications that require linking a bank account for payments, like Amazon, to analyze a client's financial state
          programmatically via the linking of their bank and investment accounts.
        </p>
      </div>

      <div class="card">
        <h4>Custom CRM Extensions</h4>
        <hr>
        <p>Most CRMs can have extensions built to make them feel more like Salesforce, by leveraging its API.
        With work, this makes it possible to program alerts, sort inbound leads, and automate many otherwise manual interactions between
        all employees and your CRM. These opportunities exist with almost any platform you may use in your day-to-day, not just CRMs.
        </p>
      </div>
    </div>

    <hr>

    <h3>Contact Nick and Links</h3>
    <ul class="footer-links">
      <li><a href="https://www.linkedin.com/in/nicholas-sandomeno-5858b5125/" target="_blank" rel="noopener">LinkedIn</a></li>
      <li><a href="https://github.com/Nsandomeno" target="_blank" rel="noopener">Github</a></li>
      <li><a href="https://twitter.com/NickSandomeno" target="_blank" rel="noopener">Twitter</a></li>
      <li><a>nick@fulminologylabs.co</a></li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HomePage',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.highlights {
  display: flex;
  justify-content: space-around;
  padding: 8px;
}
.card {
  width: 35%;
  border-radius: 8px;
  border: 2px solid black;
  box-shadow: 5px 10px #f7a943;
}
.footer-links {
  display: flex;
  justify-content: space-around;
}

h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #f7a943;
  font: bold;
}

@media screen and (max-width: 768px) {
  .highlights {
    display: flex;
    justify-content: space-between;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    padding: 0;
  }
  .footer-links {
    display: flex;
    flex-direction: column;
  }
  h3 {
    margin: 8px 0 0;
  }
  li {
    display: inline-block;
    margin: 0 4px;
  }
  .card {
    height: 100%;
    width: 60%;
    border-radius: 2px;
    border: 2px solid black;
    box-shadow: none;
    margin-bottom: 10px;
  }
}
</style>
