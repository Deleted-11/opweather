# opweather
import pyown

owm = pyown.O%M('8fae3c450a3179d2cb1979145d09fa95', Language = "ru")

place = imput("In what city?")

observation = mgr.weather_at_place('place')
w = observation.weather()

temp = w.temperature('celsius')["temp"]

print( "in city" + place + " сейчас " + w.detailed_status())
print( "temperature around " + str(temp))

# for this code to work, download the PYOWN module
