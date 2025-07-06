# AGENT GOOGLE MAPS

### **OVERVIEW**

#### Langgraph

- https://langchain-ai.github.io/langgraph/tutorials/get-started/1-build-basic-chatbot/
- https://langchain-ai.github.io/langgraph/tutorials/get-started/2-add-tools/
- https://langchain-ai.github.io/langgraph/tutorials/get-started/3-add-memory/

---

#### Google Maps API

**Google Text Search API** returns information about a set of places based on a string

The service responds with a list of places matching the text string and any location bias that has been set.

https://developers.google.com/maps/documentation/places/web-service/text-search

Take a look at the `X-Goog-FieldMask header` allows to choose exactly which fields the API will return based on your query. In the example below, I selected:

```py
"X-Goog-FieldMask": places.id
                    places.attributions 
                    places.displayName
                    places.formattedAddress
                    places.location
                    places.googleMapsLinks
```

Note that: `places.id` can be useful in your application to call other APIs, such as the one for embedding maps: 
https://developers.google.com/maps/documentation/embed/embedding-map

---

Full documentation for the Google Maps Places API:

https://developers.google.com/maps/documentation/places/web-service#features-for-places-api-new

---

### **AUTHOR**

Giovane Hashinokuti Iwamoto - Computer Science - Brazil

I am always open to receiving constructive criticism and suggestions for improvement in my developed code. I believe that feedback is an essential part of the learning and growth process, and I am eager to learn from others and make my code the best it can be. Whether it's a minor tweak or a major overhaul, I am willing to consider all suggestions and implement the changes that will benefit my code and its users.