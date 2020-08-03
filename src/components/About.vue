<template>
  <div class="wrapper">

    <div class="left-column">
      <div id='container'>
        <div class="logo-image">
          <img class="logo" src="../assets/logo.png">
        </div>

        <div class="back-button">&nbsp;<&nbsp;</div>

        <div class="card">
          <div class="card-title">VUE LTE</div>
          <div class="node-cms">Node CMS</div>

          <div class="project-id">
            Project ID: 234
            <button class="btn view">view on</button>
          </div>
          <div class="auto-deploy">
            Auto Deploy
            <label class="switch">
              <input type="checkbox" checked>
              <span class="slider round"></span>
            </label>
          </div>
          <div class="slack-notifications">
            Slack Notifications
            <label class="switch">
              <input type="checkbox">
              <span class="slider round"></span>
            </label>
          </div>

        </div>

        <div class="card-footer-buttons">
          <button class="rollback">Rollback</button>
          <button class="deploy-now">Deploy Now</button>
        </div>

        <div class="footnote">ARCHIVE PROJECT</div>
      </div>
    </div>

    <div class="right-column">
      <div class="dploy-script-title">
        <div class="title">DPloy Script</div>
        <input type="button" class="edit-script" value="Edit Script">
      </div>

      <div class="script">git pull origin master<br/>
          composer install --no-interaction --prefer-dist --optimize-autoloader<br/>
          echo ''  '' | sudo -S service php7.3-fpm reload<br/><br/>

          if [ -f artisan ]<br/>
          then<br/>
          &nbsp;&nbsp;&nbsp;php artisan migrate --force<br/>
          &nbsp;&nbsp;&nbsp;php artisan horizon:terminate<br/>
          fi<br/><br/>
          yarn<br/>
          yarn prod<br/><br/>

          if [ -f artisan ]<br/>
          then<br/>
          &nbsp;&nbsp;&nbsp;php artisan migrate --force
          &nbsp;&nbsp;&nbsp;php artisan horizon:terminate<br/>
          fi<br/>
      </div>

      <div class="deployment-title">
        <div class="title">Deployments</div>
        <input type="button" class="view-deploy-history" value="View Deployment History">
      </div>

      <div class="deployment-tabs">
        <div class="deployment-hist-left-tab">Froddo Baggins
          <div class="left-timestamp">
            15:52 | 23 Aug&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✓
          </div>

          <div class="subtext">
            Commit Details Lorem ipsum dolor<br/> sit amet lorem ipsul dolor<br/> sit amet amet amet amet.
          </div>

          <input type="button" class="colorcode-button" value="#7a7df2e">
        </div>

        <div class="deployment-hist-right-tab">Bilbbo Baggins
          <div class="left-timestamp">
            15:52 | 23 Aug&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;✓
          </div>

          <div class="subtext">
            Commit Details Lorem ipsum dolor<br/> sit amet lorem ipsul dolor<br/> sit amet amet amet amet.
          </div>

          <input type="button" class="colorcode-button" value="#7a7df2e">
        </div>
      </div>

      <div class="builds-title">
        <div class="title">Builds</div>
      </div>

      <input type="input" class="builds-history" value="There is currently no build history">

      <div class="deployment-title">
        <div class="title">Sentry Issues</div>
        <input type="button" class="view-deploy-history" value="View on Sentry">
      </div>

      <div class="table">
        <div class="left-table-column">
          <table>
            <thead>
              <tr class="no-back">
                <th></th>
                <th>USERS AFFECTED</th>
                <th>EVENTS</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td>UnhandledRejection</td>
                <td>265</td>
                <td>265</td>
              </tr>
              <tr>
                <td>UnhandledRejection</td>
                <td>265</td>
                <td>265</td>
              </tr>
              <tr>
                <td>UnhandledRejection</td>
                <td>265</td>
                <td>265</td>
              </tr>
              <tr>
                <td>UnhandledRejection</td>
                <td>265</td>
                <td>265</td>
              </tr>
              <tr>
                <td>UnhandledRejection</td>
                <td>265</td>
                <td>265</td>
              </tr>
            </tbody>
          </table>
        </div>

        <div class="right-table-column">
          <div class="users-affected">
            <h1>52</h1>
            <div class="users-affected-subtext">USERS AFFECTED</div>
          </div>

          <div class="users-affected">
            <h1>102</h1>
            <div class="users-affected-subtext">ERRORS</div>
          </div>
        </div>
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: 'About'
}
</script>
<style>
.wrapper {
    height: 1580px;
    background-color: #11151E;
    width:100%;
    position: relative;
    z-index: -4;
}

.back-button {
    background-color: #262B3A;
    border-radius: 10px;
    border: none;
    color: #637191;
    padding: 10px 20px;
    text-align: left;
    text-decoration: none;
    font-size: 16px;
    margin: 85px 0 0px 10px;
    width: 60px;
    display: inline-block;
    float: left;
}

.card-footer-buttons {
    display: inline-block;
    float: left;
    margin: 480px 0 20px 5px;
}

#container {
  position: relative;
}

.footnote {
margin: 110px 0 0 0;
display: inline-block;
font-size: 12px;
font-weight: bold;
}

.deploy-now {
background-color: #4CAF50; /* Green */
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
    background-color: transparent;
    color: white;
    border: 2px solid white;
    border-radius: 10px;
    width: 190px;
}

.view {
  border: 1px white solid;
  color: white;
  cursor: pointer;
  float: right;
  border-radius: 10px;
}

.project-id {
    background-color: #262B3A;
    border-radius: 10px;
    border: none;
    color: #637191;
    padding: 10px 20px;
    text-align: left;
    text-decoration: none;
    font-size: 16px;
    margin: 15px 10px 15px 15px;
    font-weight: 700;
}

.auto-deploy {
    background-color: #262B3A;
    border-radius: 10px;
    border: none;
    color: #637191;
    padding: 10px 20px;
    text-align: left;
    text-decoration: none;
    font-size: 16px;
    margin: 0 10px 15px 15px;
    font-weight: 700;
}

.slack-notifications {
    background-color: #262B3A;
    border-radius: 10px;
    border: none;
    color: #637191;
    padding: 10px 20px;
    text-align: left;
    text-decoration: none;
    font-size: 16px;
    margin: 0 10px 15px 15px;
    font-weight: 700;
}

.card-title {
    font-size: 30px;
    text-align: center;
    margin: 110px 0 0 0;
}

.node-cms {
    font-size: 16px;
    text-align: center;
    margin: 0;
}

.card {
    z-index: -1;
    background-color: #1D222E;
    border-radius: 10px;
    border: none;
    color: #637191;
    padding: 15px 32px;
    text-align: left;
    text-decoration: none;
    font-size: 16px;
    margin: 5px 0 30px 10px;
    float: left;
    display: flex;
    position: absolute;
    top: 137px;
    left: 0px;
    width: 380px;
    height: 450px;
    }

table {
border: none;
border-collapse: collapse;
width: 98%;
height: 330px;
margin: 0 0 0 10px;
}

td {
    border: none;
}

th {
border: none;
}

tr {
border: none;
background-color: #171B26;
}

.no-back {
background-color: transparent;
}

.table thead th {
    vertical-align: bottom;
    border-bottom: none;
    border-top: none;
}

.table td {
    padding: 0.75rem;
    vertical-align: top;
    border-top: none;
}

.table {
width: 100%;
height: 360px;
display: inline-block;
color: #637191;
}

.left-table-column {
float: left;
display: inline-block;
width: -moz-calc(100% - 250px);
width: -webkit-calc(100% - 250px);
width: calc(100% - 250px);
height: 360px;
}

.right-table-column{
float: left;
display: inline-block;
width: 250px;
height: 360px;
}

.deployment-title {
    text-align: left;
    color: #FF4D6A;
    font-size: 30px;
    margin: 0 0 0 10px
    }

    .view-deploy-history {
        float: right;
        background-color: #1D222E;
        border-radius: 10px;
        border: none;
        color: #637191;
        padding: 15px 32px;
        text-align: center;
        text-decoration: none;
        display: inline-block;
        font-size: 16px;
        margin: 5px 10px;
        cursor: pointer;
        display:inline-block;
    }

    .subtext {
    font-size: 12px;
    color: #52596d;
    float: left;
    display: inline-block;
    margin: 20px 0 0 0;
    }

.left-column {
    float:left;
    display:inline-block;
    width: 400px;
    height: 100%;
    position: relative;
}

.right-column {
    float:left;
    display:inline-block;
    width: -moz-calc(100% - 400px);
    width: -webkit-calc(100% - 400px);
    width: calc(100% - 400px);
    height: 100%;
}

.dploy-script-title {
    margin: 70px 0px 0 10px;
    text-align: left;
    color: #FF4D6A;
    font-size: 30px;
    display: flex;
    justify-content: space-between;
}

.rollback {
  pointer: cursor;
  width: 180px;
  background-color: #323846;
  border-radius: 10px;
  border: none;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
}

.builds-title {
    margin: 30px 0px 0 10px;
    text-align: left;
    color: #FF4D6A;
    font-size: 30px;
    display: flex;
    justify-content: space-between;
}

.logo {
margin: 70px 0 0 0;
}

.logo-image {
    position: absolute;
    left: 100px;
    z-index: 1;
}

.builds-history {
background-color: #151921;
  border-radius: 10px;
  border: none;
  color: #637191;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 26px;
  margin: 5px 0 30px 10px;
  float:left;
  display:inline-block;
  height:150px;
  width: 98%;
}

.script {
background-color: #1D222E;
  border-radius: 10px;
  border: none;
  color: #637191;
  padding: 15px 32px;
  text-align: left;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
    margin: 5px 0 30px 10px;
    float:left;
    display:inline-block;
    height:450px;
    width: 98%;
}

.colorcode-button {
  background-color: #323846;
  border-radius: 10px;
  border: none;
  color: #637191;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 12px;
  margin: 25px 0 0 70px;  cursor: pointer;
  float:left;
  display:inline-block;
}

.edit-script {
  background-color: #1D222E;
  border-radius: 10px;
  border: none;
  color: #637191;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 5px 10px;
  cursor: pointer;
   float:left;
    display:inline-block;
}

.deployment-hist-left-tab {
  background-color: #1D222E;
  border-radius: 10px;
  border: none;
  color: #CDDDFF;
  padding: 15px 32px;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 5px 40px 0 0;
  cursor: pointer;
  float:left;
  display:inline-block;
  height: 150px;
  width: 440px;
}

.deployment-hist-right-tab {
  border: 2px solid #FF4D6A;
  background-color: #1D222E;
  border-radius: 10px;
  color: #CDDDFF;
  padding: 15px 32px;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 5px 5px 0 5px;
  cursor: pointer;
  float:left;
  display:inline-block;
  height: 150px;
  width: 440px;
}

.title {
   float:left;
    display:inline-block;
}

.deployment-tabs {
    margin: 20px 0px 0 10px;
    text-align: left;
    font-size: 25px;
    display: inline-block;
    }

    .froddo {
    float: left;
    display: inline-block;
    }

    .bilbbo {
    float: left;
    display: inline-block;
    }

    .left-timestamp {
    float: right;
    display:inline-block;
    font-size: 12px;
    color: #52596d;
    }

    .users-affected {
    background-color: #1D222E;
    border-radius: 10px;
    border: none;
    color: #637191;
    padding: 40px 32px;
    text-decoration: none;
    display: inline-block;
    margin: 15px 0 0 15px;
    cursor: pointer;
    float: left;
    height: 150px;
    width: 90%;
    }

    .users-affected-subtext {
    font-size: 12px;
    }

    .switch {
  position: relative;
  display: inline-block;
  width: 60px;
  height: 34px;
  float: right;
}

.switch input {
  opacity: 0;
  width: 0;
  height: 0;
}

.slider {
  position: absolute;
  cursor: pointer;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background-color: #ccc;
  -webkit-transition: .4s;
  transition: .4s;
}

.slider:before {
  position: absolute;
  content: "";
  height: 26px;
  width: 26px;
  left: 4px;
  bottom: 4px;
  background-color: white;
  -webkit-transition: .4s;
  transition: .4s;
}

input:checked + .slider {
  background-color: #FF4D6A;
}

input:focus + .slider {
  box-shadow: 0 0 1px #2196F3;
}

input:checked + .slider:before {
  -webkit-transform: translateX(26px);
  -ms-transform: translateX(26px);
  transform: translateX(26px);
}

/* Rounded sliders */
.slider.round {
  border-radius: 34px;
}

.slider.round:before {
  border-radius: 50%;
}

</style>
