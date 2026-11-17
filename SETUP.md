# Set up the `karkichtn` GitHub profile

## 1. Put the files in the profile repository

The repository must be **public** and named exactly `karkichtn`.

Copy these package contents into the root of that repository:

- `README.md` -> repository root
- `.github/workflows/snake.yml` -> `.github/workflows/snake.yml`
- `assets/matrix-header.gif` -> `assets/matrix-header.gif`

Keep the folder structure exactly as shown. The README references the GIF using the relative path `assets/matrix-header.gif`.

## 2. Allow the workflow to publish the snake

In the repository, open **Settings -> Actions -> General -> Workflow permissions** and select **Read and write permissions**. Save the setting.

The workflow uses the built-in `GITHUB_TOKEN`; you do not need to create a personal access token or add a secret.

## 3. Run the animation workflow

1. Open the repository's **Actions** tab.
2. Select **Generate Matrix Contribution Snake**.
3. Click **Run workflow**.
4. After it succeeds, confirm that an `output` branch exists and contains the two generated SVG files.

The workflow also runs daily at 00:23 UTC (05:53 IST).

## 4. Confirm the profile README

Open `https://github.com/karkichtn`. GitHub displays the README when the repository is public, its name exactly matches the username, and `README.md` is in the repository root.

## Notes

- The animated Matrix banner is included locally in `assets/`, so it does not depend on an image-hosting service.
- The typing animation, stats cards, and streak card use third-party image services. Those services can occasionally rate-limit or go offline.
- The featured repository cards link only to repositories visible on the public profile at the time this package was prepared. Change or remove any card that you no longer want to feature.
- GitHub does not allow a profile README to apply custom CSS or JavaScript to the entire profile page; this package styles the README area only.
