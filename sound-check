# test_sounds.py
import pygame, os, time

pygame.mixer.init()
sounds = ["twinkling.wav", "hit.wav", "drop.wav", "lose_life.wav", "victory.wav", "game_over.wav", "bg_music.wav"]

print("Testing Christmas sounds…\n")
for s in sounds:
    path = os.path.join("assets", s)
    if not os.path.exists(path):
        print(f"Missing: {s}")
        continue
    try:
        sound = pygame.mixer.Sound(path)
        print(f"Playing {s} …")
        sound.play()
        time.sleep(1.2)           # hear each one clearly
    except Exception as e:
        print(f"Broken: {s} → {e}")

print("\nAll done! Press Enter to quit")
input()
