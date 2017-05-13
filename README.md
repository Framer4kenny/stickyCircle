# stickyCircle
sticky circle proto
```
BG = new BackgroundLayer
	backgroundColor: "white"
	contrast: 5000

layerA = new Layer
	borderRadius: "100%"
	width: 150
	height: 150
	blur: 10
	parent: BG
	backgroundColor: "aqua"
layerA.center()

layerB = new Layer
	borderRadius: "100%"
	width: 150
	height: 150
	blur: 10
	parent: BG
	backgroundColor: "aqua"
layerB.center()

layerA.states.add
	properties:
		y: Align.center(-165)

layerB.onClick ->
	layerA.states.next()
 ```
