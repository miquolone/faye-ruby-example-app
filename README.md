# Example Faye app purely in Ruby 
New to Faye & do not know how to use it in Ruby ? This is a good place to start.

## Installation 

Install dependencies 
 
    
	gem install faye evementmachine thin


Fire up Faye server 

    
	rackup faye.ru -s thin -E production


Fire eventmachine client which will respond to the browser request

    
	ruby eventmachine.rb


Open client.html in browser (since you do not have a webserver running, you can simply open up the file in browser to execute javascript)

The client will send a message & eventmachine.rb will respond to it. Both of the parties are suppose to respond instantly to the incoming message.

### Browser showing message from server
![Client showing message from server](https://dl.dropboxusercontent.com/u/76443013/Faye-browser.png)

### Server showing message from browser
![Server showing message from browser](https://dl.dropboxusercontent.com/u/76443013/Faye-eventmachine.png)


Now that you have seen Faye in action, go build your own realtime messaging app in Ruby/Rails using Faye. 
