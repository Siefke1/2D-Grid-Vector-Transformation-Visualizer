# 2D Grid & Vector Transformation Visualizer

An interactive web-based visualization tool for exploring linear transformations in 2D space. This tool displays grids as lines and allows you to input vectors and 2x2 transformation matrices to see how they affect both the grid structure and individual vectors.

## Features

- **Grid Visualization**: Display 2D grids as lines forming squares
- **Vector Input**: Input custom vectors and see them as arrows
- **Matrix Transformations**: Apply 2x2 transformation matrices

## Getting Started

1. **Open the Visualization**:
   - open `index.html` in your web browser
   - The visualization will load automatically

2. **Understanding the Display**:
   - **Blue Lines**: Original grid
   - **Red Lines**: Transformed grid
   - **Green Arrow**: Your input vector
   - **Yellow Arrow**: Transformed vector
   - **Black Lines**: Coordinate axes

## Usage

### Basic Operation

1. **Input a Vector**:
   - Enter X and Y coordinates in the "Vector Input" section
   - Click "Update Vector" to see the vector displayed as a green arrow

2. **Apply Transformations**:
   - Use preset buttons for common transformations
   - Or manually enter a 2x2 matrix and click "Apply Transformation"

3. **Adjust Grid Settings**:
   - Change grid size and spacing using the "Grid Settings" controls
   - Click "Update Grid" to apply changes

### Available Transformations

| Transformation | Matrix | Description |
|----------------|--------|-------------|
| Identity | `[1 0]`<br>`[0 1]` | No change |
| Rotation 90° | `[0 -1]`<br>`[1  0]` | Rotate 90° counterclockwise |
| Rotation 45° | `[0.707 -0.707]`<br>`[0.707  0.707]` | Rotate 45° counterclockwise |
| Scaling (2x) | `[2 0]`<br>`[0 2]` | Scale by factor of 2 |
| Shear | `[1 1]`<br>`[0 1]` | Horizontal shear |
| Reflection | `[-1 0]`<br>`[ 0 1]` | Reflect across y-axis |

## Troubleshooting

### Common Issues

1. **No visualization appears**:
   - Ensure JavaScript is enabled in your browser
   - Try refreshing the page
   - Check browser console for errors (F12)

2. **Canvas not displaying**:
   - Update your web browser to the latest version
   - Ensure HTML5 Canvas is supported

### Mathematical Background

The visualization demonstrates linear transformations using 2x2 matrices:

```
[x'] = [a b] [x]
[y']   [c d] [y]
```

Where:
- `[x, y]` is the original point/vector
- `[x', y']` is the transformed point/vector
- `[a b; c d]` is the transformation matrix

## License

This project is open source and available under the MIT License.