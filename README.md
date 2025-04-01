# defold-game-project
Main repository for a 2D game developed with Defold engine. Structured to facilitate collaboration between specialized AI agents.

# GitHub Workflow for Defold Game Project - AI Agent Collaboration

## Repository Structure
- **defold-game-project**: Main repository for game code and assets
- **defold-game-docs**: Documentation repository for guides and reference materials

## Basic Workflow

### 1. Issues
- Each AI agent works on issues assigned to their specific role
- Issues should have clear acceptance criteria and deliverables
- Use labels to categorize issues (enhancement, bug, documentation)

### 2. Branches
- Create branches from main using naming convention: `role/feature`
- Examples:
  - `game-director/vision-doc`
  - `game-designer/player-mechanics`
  - `lua-programmer/movement-system`
  - `art-director/style-guide`

### 3. Commits
- Use descriptive commit messages with role prefix
- Format: `[Role] Description of changes`
- Examples:
  - `[Game Director] Update core game loop mechanics`
  - `[Lua Programmer] Implement character controller`

### 4. Pull Requests
- Submit PRs when features are complete
- Reference the issue number in the PR description
- Include screenshots or videos for visual changes
- Provide testing instructions when applicable

### 5. Code Reviews
- At least one other AI agent should review before merging
- Focus reviews on functionality, code quality, and alignment with game vision
- Use GitHub's review features to provide specific feedback

### 6. Project Board
- Move issues through the workflow stages:
  - Todo → In Progress → Done
- Update issue status when starting or completing work
- Add comments to issues to document progress and decisions

## Role-Specific Guidelines

### Game Director
- Approves major design decisions and vision changes
- Reviews PRs that impact the overall game direction
- Maintains the game vision document
- Coordinates between different AI agent roles

### Game Designer
- Implements gameplay systems based on approved vision
- Creates detailed design documents for features
- Works closely with Lua Programmer to implement mechanics
- Tests gameplay features for balance and fun

### Lua Programmer
- Reviews all code PRs before merging
- Maintains code quality standards
- Implements technical systems and gameplay mechanics
- Optimizes performance and handles debugging

### Art Director
- Approves all visual asset PRs
- Maintains visual style consistency
- Provides feedback on UI/UX design
- Works with 2D Game Artist to implement visual elements

### 2D Game Artist
- Creates game assets following Art Director guidelines
- Organizes assets in appropriate directories
- Optimizes assets for game performance
- Implements animations and visual effects

### Audio Designer
- Creates and implements sound effects and music
- Organizes audio assets in appropriate directories
- Ensures audio quality and consistency
- Works with Lua Programmer for audio implementation

### Narrative Designer
- Creates story elements and dialogue
- Maintains narrative consistency
- Works with Game Director to align story with gameplay
- Implements text content in appropriate formats

### UI/UX Designer
- Designs user interface elements
- Creates wireframes and mockups
- Works with 2D Game Artist for visual implementation
- Ensures intuitive and accessible user experience

## GitHub Actions Automation

The repository is configured with several GitHub Actions workflows:

1. **Build Workflow**: Automatically builds the Defold project when changes are pushed
2. **Documentation Update**: Deploys documentation changes to GitHub Pages
3. **Lint and Test**: Checks code quality and runs tests
4. **Release Workflow**: Creates game builds for different platforms when tags are pushed

## Best Practices

1. **Communication**: Use issue comments for feature-specific discussions
2. **Documentation**: Update documentation alongside code changes
3. **Testing**: Test changes thoroughly before submitting PRs
4. **Incremental Development**: Break large features into smaller, manageable issues
5. **Regular Updates**: Keep the project board updated to reflect current status
6. **Version Control**: Use semantic versioning for releases (v1.0.0, v1.1.0, etc.)
