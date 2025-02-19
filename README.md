# AI Workshop Assistant Template

A modern, responsive React application template with a beautiful dark theme and blue accents. This template includes a chat interface, navigation system, and multiple pre-built pages.

## 🚀 Complete Setup Guide for Beginners

### Step 1: Fork the Repository

1. Go to the original repository on GitHub
2. Click the "Fork" button in the top-right corner
3. Wait for GitHub to create your copy of the repository
4. You now have your own version of the project in your GitHub account

### Step 2: Set Up Netlify Deployment

1. Go to [Netlify](https://www.netlify.com/)
2. Sign up or log in (you can use your GitHub account)
3. Click "Add new site" → "Import an existing project"
4. Choose "Deploy with GitHub"
5. Select your forked repository
6. Configure the build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
7. Click "Deploy site"
8. While deploying, you can set up a custom domain name:
   - Go to "Site settings" → "Domain management"
   - Click "Add custom domain"
   - Follow the instructions to set up your domain

### Step 3: Clone to Your Computer

1. Install [Git](https://git-scm.com/) if you haven't already
2. Open GitHub Desktop or Terminal
3. If using GitHub Desktop:
   - Click "File" → "Clone repository"
   - Select your forked repository
   - Choose a local path
   - Click "Clone"
4. If using Terminal:
   ```bash
   git clone https://github.com/YOUR_USERNAME/REPOSITORY_NAME.git
   cd REPOSITORY_NAME
   ```

### Step 4: Making Changes

#### Using Visual Studio Code (Recommended for Beginners)

1. Install [Visual Studio Code](https://code.visualstudio.com/)
2. Open your cloned project:
   - File → Open Folder → Select your project folder
3. Install recommended extensions:
   - ESLint
   - Prettier
   - Tailwind CSS IntelliSense

#### Common Customizations for Non-Coders

1. **Changing the Title**
   - Open `src/components/TopMenu.tsx`
   - Find:
     ```jsx
     <h1 className="text-xl sm:text-2xl font-bold...">
       AI Workshop Assistant
     </h1>
     ```
   - Change "AI Workshop Assistant" to your title

2. **Modifying Colors**
   - Open `src/App.tsx`
   - Find the background gradient:
     ```jsx
     className="flex flex-col h-screen bg-gradient-to-b from-gray-950 via-blue-950 to-gray-950"
     ```
   - Change colors using [Tailwind color values](https://tailwindcss.com/docs/customizing-colors)
   - Common colors: blue-950, indigo-950, purple-950, etc.

3. **Changing Menu Options**
   - Open `src/App.tsx`
   - Find the navigation section:
     ```jsx
     <nav className="space-y-4">
       <a href="/dashboard">Dashboard</a>
       <a href="/projects">Projects</a>
       // etc...
     </nav>
     ```
   - Change the text between `>` and `</a>`

4. **Modifying Bottom Buttons**
   - Open `src/components/BottomMenu.tsx`
   - Find:
     ```jsx
     <span className="text-sm sm:text-base">Button 1</span>
     ```
   - Change "Button 1" to your desired text

5. **Customizing Pages**
   - Navigate to `src/pages/`
   - Open any page file (e.g., `Dashboard.tsx`)
   - Find and modify the title and content sections

#### Using bolt.new (Alternative Online Editor)

1. Go to [bolt.new](https://bolt.new)
2. Create a new project
3. Import your GitHub repository
4. Make changes directly in the browser
5. Commit and push changes from the web interface

### Step 5: Updating Your Site

#### Using Visual Studio Code

1. Save all your changes
2. Open the Source Control panel (Ctrl+Shift+G or Cmd+Shift+G)
3. Enter a commit message describing your changes
4. Click the checkmark to commit
5. Click the "..." menu and select "Push"

#### Using GitHub Desktop

1. Save all your changes
2. Open GitHub Desktop
3. Review your changes
4. Add a commit message
5. Click "Commit to main"
6. Click "Push origin"

### Viewing Your Deployment

1. Go to [Netlify](https://app.netlify.com/)
2. Select your site
3. Click "Deploys" to see deployment status
4. Your site will automatically update after each push
5. View deployment progress at: `https://app.netlify.com/sites/YOUR-SITE-NAME/overview`

## ⚙️ Environment Setup

Create a `.env` file in your project root:
```
VITE_OPENAI_API_KEY=your_openai_api_key_here
VITE_OPENAI_ASSISTANT_ID=your_assistant_id_here
```

To get these values:
1. Go to [OpenAI](https://platform.openai.com/)
2. Create an account or log in
3. Go to API section to get your API key
4. Create an Assistant to get the Assistant ID

## 🆘 Troubleshooting

Common issues and solutions:

1. **Build fails on Netlify**
   - Check if all environment variables are set in Netlify's dashboard
   - Verify the build command and publish directory

2. **Changes not showing up**
   - Make sure you committed and pushed your changes
   - Check Netlify's deploy log for errors
   - Clear your browser cache

3. **Local development issues**
   - Run `npm install` to update dependencies
   - Verify your `.env` file exists and has correct values
   - Check console for error messages

## 📄 License

MIT License - feel free to use this template for any purpose!
