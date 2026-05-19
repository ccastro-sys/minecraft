from mcpi.minecraft import Minecraft
import time

mc = Minecraft.create()

def chicken_rain():
    x, y, z = mc.player.getPos()
    # Spawns 10 chickens 10 blocks above the player
    mc.spawnEntity(x, y + 10, z, "chicken")

# Type "rain" in the game chat to trigger the code
while True:
    time.sleep(1)
    # Add your chat detection logic here
