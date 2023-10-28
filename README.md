# Backend_Notes

First step----
npm init
npm i express dotenv
"start":"node index.js"
 "type": "module",

Second step----
cors - do not allow anyone to the house ,whitelist to only this url to acess the data from server
poxy is one of solution of cors
 server:{
    proxy:{
      '/api':'http://localhost:4000',
    },
  },


Third Step------------------
online IDE  - stackBlitz,github codeSpace
user.model.js
import mongoose from "mongoose"
const userSchema = new mongoose.Schema({},{timestamps:true})
export const User = mongoose.model("User",userSchema)


