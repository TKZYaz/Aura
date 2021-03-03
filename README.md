# Aura
“Phase 1 base code”
Shall set-up the Raspberry Pi and configure it for the project
• Shall demonstrate basic understanding of Python coding
o Create simple unit conversion program
• Shall demonstrate basic understanding of Raspberry Pi I/O
o Configure LED on breadboard
o Blink LED
• Shall demonstrate basic understanding of pygame
o Add a random rectangle to the center of the game screen
o Add random ball to the top-left corner of the game screen
o Add text to the top-right of the game screen
"""
Milestone C - Software Design and Integration
Lesson 0:
Blank Pygame Template with Raspberry Pi GPIO
"""
import pygame
#import RPi.GPIO as GPIO import time
# Definitions
# Initialize Pygame pygame.init()
# Set the width and height of the screen [width, height] size = (600, 480)
screen = pygame.display.set_mode(size) pygame.display.set_caption("My Game")
# Set main loop complete complete = False
# Set the speed of loops clock = pygame.time.Clock()
# -------- Main Program Loop ----------- while not complete:
# -- Main event loop
for event in pygame.event.get():
if event.type == pygame.QUIT: complete = True
# - Add game logic should go here
# - Screen clearing code goes here screen.fill((0,0,0))
# - Draw objects on the screen

 # - Update the screen with our drawing pygame.display.flip()
# Set frame rate clock.tick(30)
# Close the window and quit. pygame.quit()
