# Moments - Personal Diary App

Moments is a personal diary app developed in Swift, utilizing programmatic UI without Storyboards. The app allows users to create, view, and manage personal posts with text and images. It features a dynamic interface powered by `UITableViewDiffableDataSource`, and uses delegates and closures for efficient data handling.

## Features

- **Main Screen with Personal Posts:**
  - Displays a list of posts, each capable of containing text and up to 4 images.
  - Text is truncated to 5 lines on the main screen, with a maximum of 2 images shown.
  - Add new posts using the "+" button in the navigation bar.

- **Detailed Post Screen:**
  - View full text and images of a post.
  - Edit or delete posts with changes reflected on the main screen.
  - Confirmation prompt before deleting a post.

- **Post Creation Screen:**
  - Add or edit post text and select images from the gallery.
  - Limit of 4 images per post with an option to remove selected images.
  - Save or cancel post creation/editing.

## Technical Details

- **Main Screen:**
  - Implemented with `UITableView` and `UITableViewDiffableDataSource`.
  - Custom `UITableViewCell` displays post content with a date, text, and images.
  - Use `UICollectionView` within cells for image display.

- **Detailed Screen:**
  - Utilizes `UIScrollView` to display detailed post contents.
  - Dynamic image grid layout based on the number of images.

- **Post Creation Screen:**
  - Uses `UITextView` for text input and `UICollectionView` for image management.
  - `UIImagePickerController` for image selection, with modal presentation.

- **Navigation:**
  - `UINavigationController` for push transitions between screens.
  - Modal transition for post creation and editing.
  - Delegates and closures for data updates across screens.

## Getting Started
Launch the app to view existing posts or create new ones.
Tap on a post to view its details or edit content.
Use the "+" button to add new posts, and manage images directly from your gallery.
