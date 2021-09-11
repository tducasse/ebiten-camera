# ebiten-camera
A simple camera library for ebiten

## Usage
```go
import camera "github.com/tducasse/ebiten-camera"

myCamera := camera.Init(screenWidth, screenHeight)
world := ebiten.NewImage(worldWidth, worldHeight)

ebiten.SetWindowSize(screenWidth*windowScale, screenHeight*windowScale)

// in your Draw call
world.Clear()
// your draw calls go here, but target world instead of screen
player.Draw(world)
// then draw the world onto the screen
myCamera.Draw(world, screen)
```