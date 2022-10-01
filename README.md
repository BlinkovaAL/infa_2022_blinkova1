# infa_2022_blinkova1
import pygame
from pygame.draw import *
pygame.init()
FPS=30
screen = pygame.display.set_mode((1000, 800))
rect(screen, 'cyan', (0, 0, 1000, 400))
rect(screen, 'yellow', (0, 550, 1000, 300))
rect(screen, 'blue', (0, 400, 1000, 155))
circle(screen, 'yellow', (900, 100), 80)
#облако 1
circle(screen, 'white', (450, 90), 50)
circle(screen, 'black', (450, 90), 50, 1)
circle(screen, 'white', (490, 90), 50)
circle(screen, 'black', (490, 90), 50, 1)
circle(screen, 'white', (420, 115), 50)
circle(screen, 'black', (420, 115), 50, 1)
circle(screen, 'white', (460, 120), 50)
circle(screen, 'black', (460, 120), 50, 1)
circle(screen, 'white', (500, 120), 50)
circle(screen, 'black', (500, 120), 50, 1)
circle(screen, 'white', (530, 90), 50)
circle(screen, 'black', (530, 90), 50, 1)
circle(screen, 'white', (550, 120), 50)
circle(screen, 'black', (550, 120), 50, 1)
#облако 2
circle(screen, 'white', (200, 100), 30)
circle(screen, 'black', (200, 100), 30, 1)
circle(screen, 'white', (230, 100), 30)
circle(screen, 'black', (230, 100), 30, 1)
circle(screen, 'white', (180, 112), 30)
circle(screen, 'black', (180, 112), 30, 1)
circle(screen, 'white', (205, 115), 30)
circle(screen, 'black', (205, 115), 30, 1)
circle(screen, 'white', (235, 115), 30)
circle(screen, 'black', (235, 115), 30, 1)
circle(screen, 'white', (260, 100), 30)
circle(screen, 'black', (260, 100), 30, 1)
circle(screen, 'white', (270, 115), 30)
circle(screen, 'black', (270, 115), 30, 1)
#облако3
ellipse(screen, 'white', (120, 220, 80, 45))
ellipse(screen, 'black', (120, 220, 80, 45), 1)
ellipse(screen, 'white', (150, 220, 80, 45))
ellipse(screen, 'black', (150, 220, 80, 45), 1)
ellipse(screen, 'white', (90, 235, 80, 45))
ellipse(screen, 'black', (90, 235, 80, 45), 1)
ellipse(screen, 'white', (130, 240, 80, 45))
ellipse(screen, 'black', (130, 240, 80, 45), 1)
ellipse(screen, 'white', (170, 240, 80, 45))
ellipse(screen, 'black', (170, 240, 80, 45), 1)
ellipse(screen, 'white', (180, 220, 80, 45))
ellipse(screen, 'black', (180, 220, 80, 45), 1)
ellipse(screen, 'white', (210, 240, 80, 45))
ellipse(screen, 'black', (210, 240, 80, 45), 1)
#море
ellipse(screen, 'blue', (-60, 535, 80, 30))
ellipse(screen, 'blue', (100, 535, 80, 30))
ellipse(screen, 'yellow', (20, 542, 80, 30))
ellipse(screen, 'blue', (260, 535, 80, 30))
ellipse(screen, 'yellow', (180, 542, 80, 30))
ellipse(screen, 'blue', (420, 535, 80, 30))
ellipse(screen, 'yellow', (340, 542, 80, 30))
ellipse(screen, 'blue', (580, 535, 80, 30))
ellipse(screen, 'yellow', (500, 542, 80, 30))
ellipse(screen, 'blue', (740, 535, 80, 30))
ellipse(screen, 'yellow', (660, 542, 80, 30))
ellipse(screen, 'blue', (900, 535, 80, 30))
ellipse(screen, 'yellow', (820, 542, 80, 30))
ellipse(screen, 'blue', (1060, 535, 80, 30))
ellipse(screen, 'yellow', (980, 542, 80, 30))
polygon(screen, 'yellow', [(880,100), (920, 100), (900, 3), (880, 100)])
polygon(screen, 'red', [(100, 500), (200, 450), (300, 500), (100, 500)])
rect(screen, 'orange', (195, 500, 10, 200))
line(screen, '#592D00', [200, 450], [120, 500])
line(screen, '#592D00', [200, 450], [150, 500])
line(screen, '#592D00', [200, 450], [180, 500])
line(screen, '#592D00', [200, 450], [210, 500])
line(screen, '#592D00', [200, 450], [240, 500])
line(screen, '#592D00', [200, 450], [270, 500])
pygame.display.update()
clock= pygame.time.Clock()
finished=False
while not finished:
    clock.tick(FPS)
    for event in pygame.event.get():
        if event.type == pygame.QUIT:
            finished = True
pygame.quit()
