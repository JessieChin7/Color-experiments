# Color-experiments
### `Color_experiment2.ipynb` 
* `plotLAB(output, draw_polygon=True, marker='o')`
    * input the model output results（LAB points，L = 50）
    * draw the polygon by `ConvexHull` in CIELAB 3D space
    * plot the points in CIELAB 3D space
    * change the marker in situation
* `convert_colors(color_codes, to_lab=True)`
    * input the color_codes（or color charts）like this:
    ```
    ['#424B54', '#93A8AC', '#FFFFFF', '#E2B4BD', '#9B6A6C']
    ```
    * covert it into RGB or LAB numpy array
    ```
    [[ 3.14174857e+01 -1.36792459e+00 -6.53942015e+00]
    [ 6.74164112e+01 -6.43887144e+00 -4.52472735e+00]
    [ 1.00000000e+02 -2.45493786e-03  4.65342115e-03]
    [ 7.75713669e+01  1.80006547e+01  1.79270892e+00]
    [ 4.99306188e+01  1.98936707e+01  6.82788001e+00]]
    ```
* `plot_lab_plane(ax, L=50, a_range=(-128, 127, 100), b_range=(-128, 127, 100))`
    * plot the surface（e.g. L=50）
* `set_lab_color_space(ax)`
    * sets the CIELAB color space for a given 3D axis object
    
