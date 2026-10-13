# Team Manager for WordPress

A lightweight WordPress plugin to manage and display team members with a responsive grid layout.

## Features

- Simple team member management interface
- Department taxonomy for organization
- Responsive CSS Grid layout
- Profile image support via Featured Image
- Contact fields (email, website)
- Shortcode with department filtering and limit support
- Transient caching for performance
- REST API compatible
- Translation ready

## Requirements

- WordPress 6.9+
- PHP 8.3+

## Installation

1. Upload the plugin folder to `/wp-content/plugins/`
2. Activate via the Plugins menu
3. Access team management under Users > Team Members

## Usage

### Managing Departments

1. Go to Users > Team Members
2. Click "Manage Departments"
3. Add your departments

### Adding Team Members

1. Go to Users > Team Members
2. Click "Add New Member"
3. Fill in:
   - Full Name
   - Department(s)
   - Email (optional)
   - Website (optional)
   - Featured Image for profile photo
4. Click Publish

### Display Settings

1. Go to Users > Team Members
2. Click "Display Settings"
3. Configure:
   - Members per row (1-6)
   - Gap between members (0-100px)
4. Save Settings

### Displaying Team Members

Use the shortcode in any post, page, or widget:

```
[team_members]
[team_members department="engineering"]
[team_members department="engineering,design" limit="6"]
[team_members limit="4"]
```

| Attribute | Description | Default |
|-----------|-------------|---------|
| `department` | Filter by department slug(s), comma-separated | all |
| `limit` | Maximum number of members to display | all |

### Reordering Members

Set the display order via the "Order" field in the Page Attributes box when editing a team member. Lower numbers appear first.

<!-- OPENWPCLUB_SPONSORS_START -->
## Open-source supporters

These companies help keep Open WP Club plugins free and maintained.

<a href="https://openwpclub.com/sponsors/"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openwpclub.com/sponsorship/supporters-dark.png"><img src="https://openwpclub.com/sponsorship/supporters.png" alt="Open WP Club supporters" width="960"></picture></a>

## Sponsored placements

Clearly labelled promotional campaigns, separate from our supporters.

<a href="https://openwpclub.com/advertise/"><picture><source media="(prefers-color-scheme: dark)" srcset="https://openwpclub.com/sponsorship/repos/team-manager-wordpress/campaigns-dark.png"><img src="https://openwpclub.com/sponsorship/repos/team-manager-wordpress/campaigns.png" alt="Open WP Club sponsored placements" width="960"></picture></a>

[Support our work](https://openwpclub.com/sponsors/) · [Discuss a campaign](https://openwpclub.com/advertise/)
<!-- OPENWPCLUB_SPONSORS_END -->

## License

GPL v2 or later
