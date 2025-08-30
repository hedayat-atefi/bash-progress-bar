# Bash Progress Bar

A simple Bash script to display a progress bar while processing files. This script searches for files matching `*cache` in the current directory and its subdirectories, then processes each file while updating a progress bar in the terminal.

## Features

- Recursively finds files ending with `cache`
- Displays a dynamic progress bar in the terminal
- Simulates file processing with a delay (customizable)

## Usage

1. **Make the script executable:**

   ```sh
   chmod +x progress-bar
   ```

2. **Run the script:**

   ```sh
   ./progress-bar
   ```

   The script will output the number of files found and show a progress bar as it processes each file.

## Customization

- Modify the `proccess-file` function in [`progress-bar`](progress-bar) to perform actual file processing instead of the simulated `sleep`.

## Example Output

```bash
finding files
find 36 files
[||||||||||||||||||||||||||||||||||||||||||||||||||] 36/36 (100%)
```

## Project Structure

```bash
progress-bar         # Main script
bar/                 # Example directory containing cache files
baz/
foo/
```

## License
