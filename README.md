# Mobile Web Specialist Certification Course

## Project Overview: Stage 1

For the **Restaurant Reviews** project, incrementally convert a static webpage to a mobile-ready web application.

**Stage One**, take a static design that lacks accessibility and convert the design to be responsive on different sized displays and accessible for screen reader use. Also, add a service worker to begin the process of creating a seamless offline experience for users.

### What do I do from here?

1. Explore the provided code, and start making a plan to implement the required features in three areas: responsive design, accessibility and offline use.

2. Write code to implement the updates to get this site on its way to being a mobile-ready website.

## Mapbox API Key

My Mapbox API key is loaded in the HTML file. The token/key is referenced throughout the app with the
variable name `mapboxApiKey`.

**index.html**

```html
<script type="application/javascript" src="js/mapbox-key.js"></script>
```

**js/mapbox-key.js**

```js
const mapboxApiKey = "<MAPBOX API KEY HERE>";
```

### Project Rubric

Your project will be evaluated by a Udacity code reviewer according to the [Restaurant Reviews project rubric](https://review.udacity.com/#!/rubrics/1090/view). Please review for detailed project requirements. The rubric should be a resource you refer to periodically to make sure your project meets specifications.

### tabindex

- Use tabindex=0 to include an element in the natural tab order of the content, but remember that an element that is focusable by default may be an easier option than a custom control

- Use tabindex=-1 to give an element programmatic focus, but exclude it from the tab order of the content

- Avoid using tabindex=1+ as much as possible. If you do use tabindex, restrict it to custom interactive controls like buttons, tabs, dropdowns, and text fields; that is, elements the user might expect to provide input to.

## Project 1 Feedback todo:

You need to implement tabindex in restaurant.html which will help the focus to be appropriately managed.

It is important that the breadcrumb is inside a _nav_ element because its purpose is navigation.

The map needs an appropriate ARIA role which explains that it is an application inside the website.

The restaurant's name in restaurant.html has a semantic mistake because it has h1 and the website's title that has a higher semantic importance also has h1. Therefore, the restaurant's name in restaurant.html needs to have a heading tag that has lower importance like h2.

When available in the browser, the site uses a service worker to cache responses to requests for site assets. Visited pages are rendered when there is no network access.

No service worker is being registered.
