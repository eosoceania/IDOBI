# IDOBI
This is a React App that allows you to connect to the IPFS network and immutably store files on the blockchain.

## Setup IPFS Gateway

https://docs.ipfs.io/introduction/install/

https://docs.ipfs.io/introduction/usage/

Initintalize
$ipfs init

Check

$ipfs help

Run daemon

$ipfs daemon

Check

$ipfs swarm

## Deal with EDITOR var bullshit

Find editor (e.g. nano)

$which nano

->/bin/nano

Set ENV

$echo export EDITOR="/bin/nano"

## Deal with CORS bullshit

$ipfs config editor

Make sure you got this going on

`(...)
  "API": {
    "HTTPHeaders": {
      "Access-Control-Allow-Methods": [
        "PUT",
        "GET",
        "POST"
      ],
      "Access-Control-Allow-Origin": [
        "*"
      ]
    }
  }
(...)`

Rerun deamon

$ipfs daemon

## Run App

$npm install

$npm start

You should have frontend running on localhost:3000 and make sure IPFS is doing its thing on :5001

Upload a file and watch magic happen - You should get file hash back

## Debug

If nothing work use dirty.html to quickstart via CDN

Check console for CORS and 403 errors.







