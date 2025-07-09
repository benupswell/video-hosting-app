# Video Hosting App

A simple video hosting application that allows you to host video files online and use them in other applications.

## Features

- Clean, responsive video player interface
- Video file information display (size, duration)
- Hosting URL examples for integration
- Mobile-friendly design

## Deployment

This app is designed to be deployed on [Netlify](https://netlify.com) for easy hosting and CDN distribution.

### Netlify Deployment

1. Push this repository to GitHub
2. Connect your GitHub repository to Netlify
3. Deploy with default settings
4. Your video will be available at: `https://your-app-name.netlify.app/assets/videos/video.mp4`

## Usage in Other Applications

Once deployed, you can use the hosted video URL in your applications:

```javascript
// Example usage in React
const videoSrc = "https://your-app-name.netlify.app/assets/videos/video.mp4";

return (
  <video controls>
    <source src={videoSrc} type="video/mp4" />
  </video>
);
```

## File Structure

```
video-hosting-app/
├── index.html          # Main HTML file with video player
├── assets/
│   └── videos/
│       └── video.mp4    # Your video file
├── .gitignore
└── README.md
```

## Local Development

Simply open `index.html` in your web browser to view the video player locally.

## Video File Management

- Place your video files in the `assets/videos/` directory
- Update the `src` attribute in `index.html` to point to your video file
- The app will automatically display video information and provide hosting URLs

## Browser Support

- Modern browsers with HTML5 video support
- Mobile browsers with playsinline support
- Progressive enhancement for older browsers 