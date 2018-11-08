# Specifications

## User Stories

### Users types:

* Decision maker \(like Coredevs, dapp devs, miners, exchanges – network stakeholder\)
* Influencer
* Editor

Each sprint is 2 weeks. Development starts: Nov 12, 2018 \(week 46\)

## Sprint 0

* Initial design \(v1\)
* Research
* Github auto-deploy of the EIP list

## Sprint 1

Goal: create website that will show list of EIPs from Github with realtime updates

* Design v2
* Create development and staging environments
* Setup deployment and testing tools
* Create worker that get EIPs data via github API

## Sprint 2

Goal: give influencers possibility to vote with their stances

* Create interface that will allow community to vote by adding link to twitter / medium / etc post \(public no sign in\)
* Create worker that will get data from media posts and check if posts are available for public
* Create worker that will dump database with influencer stances to some public github repository
* Admin portal for moderating community requests.

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>As</b>
      </th>
      <th style="text-align:left"><b>I’d like to</b>
      </th>
      <th style="text-align:left"><b>In order to</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">DM</td>
      <td style="text-align:left">
        <p>See the community feedback to Props by</p>
        <ul>
          <li>Seeing the list of proposals (EIPs parsed from github)</li>
          <li>Filter Props by Status and Category</li>
          <li>See individual stances</li>
          <li>Seeing overall statistics</li>
        </ul>
      </td>
      <td style="text-align:left">Make decisions on forking</td>
    </tr>
    <tr>
      <td style="text-align:left">Editor</td>
      <td style="text-align:left">Edit/hide proposals</td>
      <td style="text-align:left">Maintain the quality of the info</td>
    </tr>
    <tr>
      <td style="text-align:left">DM</td>
      <td style="text-align:left">Participate in open coin votings to Props</td>
      <td style="text-align:left">Inform the community</td>
    </tr>
    <tr>
      <td style="text-align:left">DM</td>
      <td style="text-align:left">Participate in open gas votings to Props</td>
      <td style="text-align:left">Inform the community</td>
    </tr>
    <tr>
      <td style="text-align:left">Editor</td>
      <td style="text-align:left">Update Stances for influencers and necessary Substantiation (any link
        like a tweet or reddit post)</td>
      <td style="text-align:left">Inform Decision Makers</td>
    </tr>
    <tr>
      <td style="text-align:left">Influencer</td>
      <td style="text-align:left">Hide own specific posts</td>
      <td style="text-align:left">Updated their stances</td>
    </tr>
    <tr>
      <td style="text-align:left">DM</td>
      <td style="text-align:left">Initiate the voting</td>
      <td style="text-align:left">Collect feedback</td>
    </tr>
  </tbody>
</table>## Sprint 3

Goal: give voters the possibility to vote with their balances on their ethereum wallets

* Create interface for voters where they can put their eth address and vote for or against the EIP \([voting mechanics](https://ethsignals.gitbook.io/wiki/~/edit/drafts/-LQnnldqUudx1pc6TfBF/specs/coin-vote-mechanics)\)
* Create worker that will get information about balance on the wallet through ethereum full node 
* Show statistics about voting on the website
* Publish on beta.tennagraph.com

## Sprint 4

Goal: connect stock.it gas voting and go to production

* Add stock.it gas voting 
* Security testing
* Performance testing
* Deploy to production

## Buffer - 2 weeks

“Give me six hours to chop down a tree and I will spend the first four sharpening the axe.”





## Old stories

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>As</b>
      </th>
      <th style="text-align:left"><b>I’d like to</b>
      </th>
      <th style="text-align:left"><b>In order to</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">DM</td>
      <td style="text-align:left">
        <p>See the community feedback to Props by</p>
        <ul>
          <li>Seeing the list of proposals (EIPs parsed from github)</li>
          <li>Filter Props by Status and Category</li>
          <li>See individual stances</li>
          <li>Seeing overall statistics</li>
        </ul>
      </td>
      <td style="text-align:left">Make decisions on forking</td>
    </tr>
    <tr>
      <td style="text-align:left">Editor</td>
      <td style="text-align:left">Edit/hide proposals</td>
      <td style="text-align:left">Maintain the quality of the info</td>
    </tr>
    <tr>
      <td style="text-align:left">DM</td>
      <td style="text-align:left">Participate in open coin votings to Props</td>
      <td style="text-align:left">Inform the community</td>
    </tr>
    <tr>
      <td style="text-align:left">DM</td>
      <td style="text-align:left">Participate in open gas votings to Props</td>
      <td style="text-align:left">Inform the community</td>
    </tr>
    <tr>
      <td style="text-align:left">Editor</td>
      <td style="text-align:left">Update Stances for influencers and necessary Substantiation (any link
        like a tweet or reddit post)</td>
      <td style="text-align:left">Inform Decision Makers</td>
    </tr>
    <tr>
      <td style="text-align:left">Influencer</td>
      <td style="text-align:left">Hide own specific posts</td>
      <td style="text-align:left">Updated their stances</td>
    </tr>
    <tr>
      <td style="text-align:left">DM</td>
      <td style="text-align:left">Initiate the voting</td>
      <td style="text-align:left">Collect feedback</td>
    </tr>
  </tbody>
</table>