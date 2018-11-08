# Roadmap & Specifications

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

EIP Navigation

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>s</b>
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
          <li>Sort By Date Created, Last Updated(Github), Last Active</li>
        </ul>
      </td>
      <td style="text-align:left">Make decisions</td>
    </tr>
  </tbody>
</table>## Sprint 2

Goal: give influencers possibility to vote with their stances

* Create interface that will allow community to vote by adding link to twitter / medium / etc post \(public no sign in\)
* Create worker that will check if posts are available for public
* Create worker that will dump database with influencer stances to some public github repository the site will then generate from.
* Admin portal for moderating community requests.
* The system should only show the most recent stance from an influencer.

Influencer Module

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
          <li>View the overall Stances</li>
          <li>See the influencers organized by stance or by rank</li>
          <li>See stances of influencers not on the list in some order (will need to
            be revisited as stances are published)</li>
          <li>See how long since that stance has been posted.</li>
        </ul>
      </td>
      <td style="text-align:left">Make decisions on forking</td>
    </tr>
    <tr>
      <td style="text-align:left">Community Member</td>
      <td style="text-align:left">
        <p>Submits stances with the following information</p>
        <ul>
          <li>Twitter Handle</li>
          <li>Stance</li>
          <li>Source</li>
          <li>Date</li>
        </ul>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Admin</td>
      <td style="text-align:left">
        <p>Signs in
          <br />Sees a Feed of Submissions</p>
        <p>Can Reject or Accept Them</p>
        <p></p>
        <p>Views the list of current stances by EIP and can edit/delete if needed.</p>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Influencer</td>
      <td style="text-align:left">
        <p>Can delete or make their stance substantiation private on their respective
          platform.</p>
        <p>Send a request to take down a response for posts they have made private
          or deleted. ( can just be an email, or a twitter DM )</p>
      </td>
      <td style="text-align:left"></td>
    </tr>
    <tr>
      <td style="text-align:left">Bot</td>
      <td style="text-align:left">The bot should check semi-regularly if the substantiation still is public,
        and if not should remove it from our site, and update the jsonDB file accordingly.</td>
      <td
      style="text-align:left"></td>
    </tr>
  </tbody>
</table>## Sprint 3

Goal: give voters the possibility to vote with their balances on their Ethereum wallets

* Create interface for voters where they can put their eth address and vote for or against the EIP \([voting mechanics](https://ethsignals.gitbook.io/wiki/~/edit/drafts/-LQnnldqUudx1pc6TfBF/specs/coin-vote-mechanics)\)
  * Yay
  * Nay
  * Abstain
* Create worker that will get information about balance on the wallet through Ethereum full node 
  * Look at how [http://carbonvote.com/](http://carbonvote.com/) does it.
* Show the statistics on the relevant EIP pages.
* Publish on beta.tennagraph.com

## Sprint 4

Goal: connect stock.it gas voting and go to production

* Add slock.it gas voting 
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