# solid-blog

`Nov 7 2022`

Today I started working on a Solid app project. I called it Solid Blog since I couldn't think of any cool name for now. This will be a simple blog app where users can log in with their Solid WebID and start writing. Their post data will be stored in their own pod. 

I just finished the login page with <LoginButton /> from `solid-react-ui`. I used the color scheme generated by [Colormind](http://colormind.io/) and icons from [Remix Design](https://github.com/Remix-Design/remixicon#usage). The <LoginButton> has two required properties: `oidcIssuer` and `redirectUrl`. `oidcIssuer` is user WebID captured through an input field or option from a select list. The `redirectUrl` is where users are directed to after they have logged in with a Solid account. To capture webID, I created two variarble (`oidcIssuer` and `podProvider`) which change states to the user input or pod option value. I also initalized a `currentUrl` variable as the root url which changes to `window.location.href` after user login. 
