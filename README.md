## Container Queries
___

### One of the requirement for using container queries is that you have to define what element is a container.
```
.cards {
    container-type: inline-size;
}
```
### Containers could also be given names. Styles inside of named container will only apply inside of that specific named container.
```
    .cards {
        container-name: cards;
    }

    @container cards (min-width: 45ch) {
        .card {
            background-color: yellow;
        }
    }
```

#### WIth container queries also come container queries lenght units. When applying styles to a container using container queries, you can use container query length units. These units specify a length relative to the dimensions of a query container. Components that use units of length relative to their container are more flexible to use in different containers without having to recalculate concrete length values.
#### cqi: 1% of a query container's inline size