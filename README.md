
# 2025_02_21_InfiniSyncableNtpLoop  

The idea is to create a game loop based on NTP time every N seconds.  

However, to avoid waiting for the next loop in real-world events, you need to be able to apply and remember an offset for the game.  
In multiplayer, there is a 5-30 ms delay when sending the reset message.  
Instead, you provide the game with the next offset NTP reset time.  

It should allows to keep the headset sync on the device clock and need only once message to sync them all for the reste of the sessions.

