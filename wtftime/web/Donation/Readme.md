# Donation
* Hint        : Save the kittens!
* URL         : http://138.68.96.149:2293
* Download    : Donation.zip

#

This is the home page of the website after we login
![WebHome](https://i.imgur.com/zZqjv8L.png)

I'm trying to look more in the zip file, and I got some injection point in the view.py, there is a simple parameters injection in donate function.

![DonateDef](https://i.imgur.com/06q4wA5.png)

We can pass a parameter in `to params` so our `to` look like this

`kitten&amount=-99999`

We can easily change the `to` values in a web browser with inspect element and it will look like this
![ChangeVal](https://i.imgur.com/6xGQjS7.png)

Donate it again one more time and we will got the flag

![Flag](https://i.imgur.com/0zrXyhZ.png)
#

Flag : flag{lo0k_at_all_the_p0llut1on}
