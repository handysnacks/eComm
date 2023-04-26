# Overview

This is an example of what you can do in techdocs.

Here is the overview page for the Digital site archive search component.

It's cool isn't it?

# Assets, links

Look at this lovely dog!

![This is a pretty cute dog](./cute-dog.png)

We can also link you to a lovely video of Backstage: [this is a lovely Backstage video](https://www.youtube.com/watch?v=85TQEpNCaU0)


# Relationship diagrams

```plantuml format="png" classes="uml myDiagram" alt="Roadie" title="Look at this! Built with plantUML" width="300px" height="300px"
  Roadie ->  Depot: loves
  Roadie <-- Depot: Returns love
```

::uml:: format="png" classes="uml myDiagram" alt="My super diagram placeholder" title="Look at this! Another diagram built with UML" width="300px" height="300px"
  Roadie ->  Costco: loves
  Roadie <-- Costco: Returns love
::end-uml::

# Code blocks

``` bash
#!/bin/bash

function doesRoadieLoveDogs(){
  return 1
}

if [ doesRoadieLoveDogs ];then
  echo "Roadie really loves dogs and the world is better for it!"
else
  echo "There is no way roadie doesn't love dogs >:("
fi

exit 1;
```
# Cloud 2.0 code blocks

''' react
const getUser = (authority: string, clientId: string) => {
  const oidcStorage = sessionStorage.getItem(
    `oidc.user:${authority}:${clientId}`
  );
  if (!oidcStorage) {
    return null;
  }

  return User.fromStorageString(oidcStorage);
};

const configureAuthLink = (authority: string, clientId: string) =>
  setContext((_, { headers }) => {
    const user = getUser(authority, clientId);
    const token = user?.access_token;
    return {
      headers: {
        ...headers,
        authorization: token ? `Bearer ${token}` : '',
      },
    };
  });
  '''