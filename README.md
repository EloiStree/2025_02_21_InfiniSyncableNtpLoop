
# Infini Syncable Ntp Loop  

The idea is to create a game loop based on NTP time every N seconds.  

However, to avoid waiting for the next loop in real-world events, you need to be able to apply and remember an offset for the game.  
In multiplayer, there is a 5-30 ms delay when sending the reset message.  
Instead, you provide the game with the next offset NTP reset time.  

It should allows to keep the headset sync on the device clock and need only once message to sync them all for the reste of the sessions.

Why I am creating that ?

I want kids to make a game triangulate in a room.
That share the exact same timing.
It won't be multiplayer network game.
But they will be able to see the same event at the same time in the space space.

But is is synchable with a simple IID message and an NTP server.


Required: 
- NTP OFFSET: https://github.com/EloiStree/OpenUPM_UnityFetchOffsetNTP.git
- TIME PCT : https://github.com/EloiStree/2025_02_17_TimePercentInterface