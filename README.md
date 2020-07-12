## Starter Project

- css provided (global styles, styled components)
- folders/files already setup
- all imports included
- index.js for easier imports

## Styled Components

[styled-components](https://styled-components.com/)

```jsx
import styled from "styled-components";

const ReactComponent = () => {
 // logic here
 return <Wrapper>
 {some content}
 </Wrapper>
}


const Wrapper = styled.htmlElement`
write your styles here
`
export default ReactComponent
```

## React Icons

[react-icons](https://react-icons.github.io/react-icons/)

```jsx
import { FiUsers, FiUserPlus } from 'react-icons/fi';
<FiUsers className='nameOfTheClass'> </FiUsers>;
```

## React Router Dom

"react-router-dom": "^5.2.0",
[react-router-dom](https://reactrouter.com/web/guides/quick-start)

- <Switch> renders the first child <Route> that matches
- A <Route path="*"> always matches

## Gihthub API

- root endpoint
  [github api root endpoint](https://api.github.com)
- get user
  [user](https://api.github.com/users/wesbos)
- user
  [ repos](https://api.github.com/users/john-smilga/repos?per_page=100)
- followers
  [followers](https://api.github.com/users/john-smilga/followers)
- rate limit
  [rate limit](https://api.github.com/rate_limit)

  For unauthenticated requests, the rate limit allows for up to 60 requests per hour. Unauthenticated requests are associated with the originating IP address, and not the user making requests.

## Fusion Charts

- Main Site
  [fusion charts](https://www.fusioncharts.com/)
- First React Chart
  [first chart](https://www.fusioncharts.com/dev/getting-started/react/your-first-chart-using-react)
- List Of Charts
  [list of charts](https://www.fusioncharts.com/dev/chart-guide/list-of-charts)
- Themes
  [themes](https://www.fusioncharts.com/dev/themes/introduction-to-themes)

## Auth0

- Main Site
  [auth0](https://auth0.com/)

- Create Application
- Choose : Single Page Web Applications
- Choose : React
- Go to Settings Tab
- Copy/Paste Domain, ClientID - can be public (or use .env)
- Add Domain -
  for now http://localhost:3000 (DON'T COPY PASTE FROM URL BAR)
  - Allowed Callback URLs
  - Allowed Logout URLs
  - Allowed Web Origins
    SAVE CHANGES!!!!!!!!!!!!!!!
- Connections
  email,social

[react sdk docs](https://auth0.com/docs/libraries/auth0-react)
[react sdk api docs](https://auth0.github.io/auth0-react/)

## Deployment

[netlify](https://www.netlify.com/)

## Additional Info

#### Redirects with react-router-dom

In order for routing to work on netlify, redirects was added to the public folder

- \_redirects file in public

```

/*    /index.html   200

```

[redirects blog post](https://dev.to/dance2die/page-not-found-on-netlify-with-react-router-58mc)

#### Warnings and create-react-app

```js
"build": "CI= react-scripts build",
```

[create-react-app warning fix](https://community.netlify.com/t/how-to-fix-build-failures-with-create-react-app-in-production/17752)
