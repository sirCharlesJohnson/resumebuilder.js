var bio = {
    "name" : "Charles Johnson",
    "role" : "Programmer",
    "contacts" : {
        "mobile": "407-234-8985",
        "email": "johcha7@yahoo.com",
        "location": "Orlando"
    },
    "welcomeMessage": "Welcome to my Live Resume!",

    "skills" : [
        "Java", " Javascript", " C++ ", " Python"
    ],
    "bioPic": "images/me.jpg"

 }  


 var education = {
    "schools": [
         {
            "name": "Everest University",
            "location": "Orlando, FL",
     	    "degree": "Bachelors", 	
            "majors": ["CIS"],
            "dates": 2014,
            "url": "http://everestuniversity.org"
        }
    ],
   "onlineCourses": [
     {
       "title": "JavaScript Basics",
       "school" : "Udacity",
       "dates": 2015,
       "url": "http://www.udacity.com/course/ud804"
     },

     {
       "title": "JavaScript Basics",
       "school" : "Treehouse",
       "dates": 2015,
       "url": "http://www.teamtreehouse.com"
     },

     {
       "title": "JavaScripts Loops, Arrays and Objects",
       "school" : "Treehouse",
       "dates": 2015,
       "url": "http://www.teamtreehouse.com"
     },

     {
       "title": "Python Basics",
       "school" : "Treehouse",
       "dates": 2015,
       "url": "http://www.teamtreehouse.com"
     },

     {
       "title": "Java Basics",
       "school" : "Treehouse",
       "dates": 2015,
       "url": "http://www.teamtreehouse.com"
     },

     {
       "title": "Java Objects",
       "school" : "Treehouse",
       "dates": 2015,
       "url": "http://www.teamtreehouse.com"
     },
     
     {
       "title": "C++, Short and Sweet",
       "school" : "Udemy",
       "dates": 2014,
       "url": "http://www.udemy.com"
     },
 
     {
       "title": "Become a Certified Web Developer",
       "school" : "Udemy",
       "dates": 2013,
       "url": "http://www.udemy.com"
     },

     {
       "title": "Creating an MP3 Player with HTML5",
       "school" : "Udemy",
       "dates": 2013,
       "url": "http://www.udemy.com"
     }	
   ],	

        	
display: function() {
for (edu in education.schools) {
$('#education').append(HTMLschoolStart);
var formattedName = HTMLschoolName.replace("%data%", education.schools[edu].name);
var formattedDegree = HTMLschoolDegree.replace("%data%", education.schools[edu].degree);
var formattedNameAndDegree = formattedName + formattedDegree;
$(".education-entry:last").append(formattedNameAndDegree);
var formattedDate = HTMLschoolDates.replace("%data%", education.schools[edu].dates);
$(".education-entry:last").append(formattedDate);
var formattedLocation = HTMLschoolLocation.replace("%data%", education.schools[edu].location);
$(".education-entry:last").append(formattedLocation);
if (education.schools[edu].majors.length > 0) {
for (major in education.schools[edu].majors) {
var formattedMajor = HTMLschoolMajor.replace("%data%", education.schools[edu].majors[major]);
$(".education-entry:last").append(formattedMajor);
}
}
}
//online classes
$('#education').append(HTMLonlineClasses)
for (online in education.onlineCourses) {
$('#education').append(HTMLschoolStart);
var formattedTitle = HTMLonlineTitle.replace("%data%", education.onlineCourses[online].title);
var formattedSchool = HTMLonlineSchool.replace("%data%", education.onlineCourses[online].school);
var formattedTitleAndSchool = formattedTitle + formattedSchool;
$(".education-entry:last").append(formattedTitleAndSchool);
var formattedDate = HTMLonlineDates.replace("%data%", education.onlineCourses[online].dates);
$(".education-entry:last").append(formattedDate);
var formattedURL = HTMLonlineURL.replace("%data%", education.onlineCourses[online].url);
$(".education-entry:last").append(formattedURL);
}
}
}

education.display();

var work = {
  "jobs": [
    {
      "employer": "Wawa",
      "title": "Facilities",
      "dates": "May 2013 - Current",
      "description": "Maintaining landscaping and interior as well."
    },
    
    {
      "employer": "Olive Garden",
      "title": "Busser",
      "dates": "April 2012 - 2013",
      "description": "Setting on clearing dining room tables as well as making sure the dining room looked good."
    },

    {
      "employer": "Valet Cleaners",
      "title": "Supervisor",
      "dates": "January 2012 - April 2012",
      "description": "Supervising co-workers to make sure the  production was completed."
    },

    {
      "employer": "Hanger Cleaners",
      "title": "Dry Cleaner",
      "dates": "Febuary 2007 - October 2012",
      "description": "Cleaning the garments."
    },
   
    {
      "employer": "Custom Cleaners",
      "title": "Dry Cleaner and Driver",
      "dates": "January 2002 - January 2007",
      "description": "Drycleaned the garments than I delivered them to drop stores."
    },

    {
      "employer": "Touch of Class Drycleaners",
      "title": "Supervisor",
      "dates": "April 1992 - December 2002",
      "description": "Supervising co-workers to make sure the  production was completed."
    
    }
  ]
}

//Display work json in resume object
function displayWork() {

for(job in work.jobs){

$("#workExperience").append(HTMLworkStart);

var formattedEmployer = HTMLworkEmployer.replace("%data%", work.jobs[job].employer);
var formattedTitle = HTMLworkTitle.replace("%data%", work.jobs[job].title);
var formattedEmployerTitle = formattedEmployer + formattedTitle;
$(".work-entry:last").append(formattedEmployerTitle);

var formattedDates = HTMLworkDates.replace("%data%", work.jobs[job].dates);
$(".work-entry:last").append(formattedDates);

var formattedDescription = HTMLworkDescription.replace("%data%", work.jobs[job].description);
$(".work-entry:last").append(formattedDescription);

};

};

displayWork();


function locationizer(work_obj) {
    var locationArray = [];

    for (job in work_obj.jobs) {
        var newLocation = work_obj.jobs[job].location;
        locationArray.push(newLocation);
    }
 
    return locationArray;
}


console.log(locationizer(work));



function inName(nameString){
var nameArray = nameString.split(" ");
var lastName = nameArray[1].toUpperCase();
var firstName = nameArray[0].toLowerCase();
firstName = firstName[0].toUpperCase() + firstName.slice(1);
return firstName + " " + lastName;
};

$("#main").append(internationalizeButton);


$(document).click(function(loc) {
  // your code goes here!
  var x = loc.pageX;
  var y = loc.pageY;

  logClicks(x,y);
});


var name = bio.name;
var formattedName = HTMLheaderName.replace("%data%", bio.name);

var role = bio.role;
var formattedRole = HTMLheaderRole.replace("%data%", role);

$("#header").prepend(formattedRole);
$("#header").prepend(formattedName);


var mobile = bio.contacts.mobile;
var formattedMobile = HTMLmobile.replace("%data%", mobile);
$("#topContacts").append(formattedMobile);

var email = bio.contacts.email;
var formattedEmail = HTMLemail.replace("%data%", email);
$("#topContacts").append(formattedEmail);

var _location = bio.contacts.location;
var formattedLocation = HTMLlocation.replace("%data%", _location);
$("#topContacts").append(formattedLocation);

var bioPic = bio.bioPic;
var formattedBioPic = HTMLbioPic.replace("%data%", bioPic);
$("#header").append(formattedBioPic);

var welcomeMessage = bio.welcomeMessage;
var formattedWelcomeMessage = HTMLWelcomeMsg.replace("%data%", welcomeMessage);
$("#header").append(formattedWelcomeMessage);

var skills = bio.skills;

if(bio.skills.length > 0) {

$("#header").append(HTMLskillsStart)

var formattedSkills = HTMLskills.replace("%data%", bio.skills[0]);
$("#skills").append(formattedSkills);
formattedSkill = HTMLskills.replace("%data%", bio.skills [1]);
$("#skills").append( formattedSkill);
formattedSkill = HTMLskills.replace("%data%", bio.skills [2]);
$("#skills").append( formattedSkill);
formattedSkill = HTMLskills.replace("%data%", bio.skills [3]);
$("#skills").append( formattedSkill);
}


