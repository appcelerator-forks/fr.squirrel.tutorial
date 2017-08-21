# Widget for display a tutorial


## Demonstration
You can test this widget on this link https://github.com/SquirrelMobile/titanium-template-tabgroup


(https://github.com/SquirrelMobile/fr.squirrel.tutorial/blob/master/animation.gif?raw=true)
## Use it

**index.js**
```javascript
var tutorial = Alloy.createWidget("fr.squirrel.tutorial",{
  indicatorSelect : {
    image: "/images/ellipseblue.png"
  },
  indicatorUnselect : {
    image: "/images/ellipseblueinactive.png"
  },
  titleBtnStart: "Suivant",
  titleBtnEnd : "Fermer",
  success : function(e){
    tutorial.close();
  }
});
```


```javascript
tutorial.setPages([
  {
    page : {
      image : "/images/photoTutorial1.jpg"
    },
    title : {
      text : "Lorem ipsum dolor.",
    },
    subtitle :{
      text : "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Phasellus sollicitudin magna eget velit aliquet, id facilisis nulla commodo. Fusce a hendrerit dolor, sed volutpat lacus.",
    },
    logo:{
      image :"/images/logo.png"
    }
  },
  {
    page : {
      image : "/images/photoTutorial2.jpg"
    },
    title : {
      text : "Curabitur scelerisque justo.",
    },
    subtitle :{
      text : "Nam viverra gravida quam varius aliquam",
    },
    logo:{
      image :"/images/logo.png"
    }
  },
  {
    page : {
      image : "/images/photoTutorial3.jpg"
    },
    title : {
      text : "Cras in tincidunt eros.",
    },
    subtitle :{
      text : "Aenean fringilla mi sit amet luctus tristique. Cras ultrices dolor non lacus bibendum tristique.",
    },
    logo:{
      image :"/images/logo.png"
    }
  }
]);
```

## Methods


```javascript
setPages(argument);
```

"argument" this argument is a collection of each page in tutorial . You can handle each data with different properties :
* "page" : this property edit the background photo of the page
* "title" : this property edit the page's title
* "subtitle" :this property edit the page's subtitle
* "logo" :this property edit the logo


##c
