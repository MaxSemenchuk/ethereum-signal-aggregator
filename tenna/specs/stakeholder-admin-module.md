# Stakeholder Admin Module

The goal of the stakeholder admin module is as users submit different substantiations we keep track of all of the "official" social accounts of those stakeholders. These could be accounts surrounding any identity whether it be for a developer, Dapp, an exchange, etc. This data is one of the portions that will be shared publicly as part of our Historic Data Transparency.

This potentially could be a "Stakeholder" object that includes and inline "accounts" class. This could be managed in the Django admin pretty easily.

sudo json

```text
 Stakeholder {
  ID : "4082"  (unique to our system)
  name : "James Hancock"
  accounts : {
      twitter: "madeof_tin",
      reddit: "madeof_tin",
      github: "madeoftin",
  }
  tags : [ "core-dev" ]
}
```

![image](https://user-images.githubusercontent.com/1226869/49208333-83121380-f385-11e8-96ea-47c988544ff6.png)

### **Interaction with the Influencer list**

The bot already crawls hive.one and populates the list and rank of influencers.  
  
IF an Influencer already Exists as a Stakeholder  
\* It is easy to verify as it can be resolved around the Twitter handle  
  
IF an Influencer does not Exist as a Stakeholder  
\* The bot can add it as a Stakeholder with the known information from Hive.one  


### Interaction with Stances Objects

Stances would be tied to the appropriate Stakeholder object. This is important as we export the data to the github JSON library. As both the Stakeholder and Stances Objects would be published, but the influencer objects will not.

### Additional GUI options

As more stances are submitted from varied sources we will need to think of new ways to display this information. The Tagging structure will be the foundation for this UI and exists independent if a Stakeholder is on the list of influencers or not.

