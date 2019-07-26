Demo app for working with [bitrix24 REST API](https://training.bitrix24.com/rest_help/index.php) 
using [pybitrix24](https://github.com/yarbshk/pybitrix24).

## Prerequisites
- you need to have a bitrix24 app with client key and client secret
- you need to have a bitrix24 user account 

## How to use

### Installation

`$ pip install bitrix24-python3-client`

### Authentication
Call `auth()` function form the code.

If the user is not logged in, they will see the authentication form. 
If the user has been or is being authenticated, the server will redirect to REDIRECT_URI with the 
initial authentication token:
 
`https://test.com/bitrix/oauth/oauth_test.php?code=<code>`

Here `code` – request token returned by the server (the token default lifetime is 30 sec).

You need to paste this token to console to continue.

See [official examples](https://training.bitrix24.com/rest_help/oauth/examles.php) to kno more.

## Features
- Authenticate in bitrix for using REST API
- Get the list of filtered deals and joined list of contacts.

