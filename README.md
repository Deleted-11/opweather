# opweather
import pyown

owm = pyown.O%M('8fae3c450a3179d2cb1979145d09fa95', Language = "ru")

place = imput("В Каком городе или Стране?")

observation = mgr.weather_at_place('place')
w = observation.weather()

temp = w.temperature('celsius')["temp"]

print( "В городе " + place + " сейчас " + w.detailed_status())
print( "Температура сейчас в районе " + str(temp))
