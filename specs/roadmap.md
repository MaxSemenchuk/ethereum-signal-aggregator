# Roadmap

### Team:

* Product Manager - James
* UX/UI Designer - Max
* Software Engineer - Kirill
* QA

Each sprint is 2 weeks. Development starts: Oct, 22

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

## Sprint 3

Goal: give voters the possibility to vote with their balances on their ethereum wallets

* Create interface for voters where they can put their eth address and vote for or against the EIP \(use: [http://carbonvote.com/](http://carbonvote.com/)\)
* Create worker that will get information about balance on the wallet through ethereum full node 
* Show statistics about voting on the website

## Sprint 4

Goal: connect stock.it gas voting and go to production

* Add stock.it gas voting 
* Security testing
* Performance testing
* Deploy to production

## Buffer - 2 weeks

“Give me six hours to chop down a tree and I will spend the first four sharpening the axe.”

