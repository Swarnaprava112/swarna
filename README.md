# swarna
swarna text
# Swarnaprava-mallick
Swarnaprava testCode
const data = {
  name: "Royal Challengers Bangalore",
  location: "Bangalore",
  player: [
    {
      name: "Faf Du Plessis",
      country: "South Africa",
      role: "Batsman",
      "price-in-crores": "7"
    },
    {
      name: "Virat Kohli",
      country: "India",
      role: "Batsman",
      "price-in-crores": "15"
    },
    {
      name: "Glenn Maxwell",
      country: "Australia",
      role: "Batsman",
      "price-in-crores": "11"
    },
    {
      name: "Mohammad Siraj",
      country: "India",
      role: "Bowler",
      "price-in-crores": "7"
    },
    {
      name: "Harshal Patel",
      country: "India",
      role: "Bowler",
      "price-in-crores": "10.75"
    },
    {
      name: "Wanindu Hasaranga",
      country: "Srilanka",
      role: "Bowler",
      "price-in-crores": "10.75"
    },
    {
      name: "Dinesh Karthik",
      country: "India",
      role: "Wicket-keeper",
      "price-in-crores": "5.5"
    },
    {
      name: "Shahbaz Ahmed",
      country: "India",
      role: "All-Rounder",
      "price-in-crores": "2.4"
    },
    {
      name: "Rajat Patidar",
      country: "India",
      role: "Batsman",
      "price-in-crores": "0.20"
    },
    {
      name: "Josh Hazlewood",
      country: "Australia",
      role: "Bowler",
      "price-in-crores": "7.75"
    },
    {
      name: "Mahipal Lomror",
      country: "India",
      role: "Bowler",
      "price-in-crores": "7.75"
    }
  ]
};

const players = data.player;

let count = 0;
let flag = false;

for (let item = 0; item < players.length; item++) {
  if (item.country !== "India") {
    count++;
  }

  if (item.role === "Wicket-keeper") {
    flag = true;
  }
}

if (count == 4) {
  console.log("There are 4 players");
} else {
  console.log("There are not exactly 4 players");
}

if(flag){
  console.log('There is one wicket keeper')
}else{
  console.log('There are no wicket player')
}
