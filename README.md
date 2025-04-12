# Codeblitz-hackathon-project
# Construction Cost Estimator

A web-based tool that helps civil engineers estimate construction costs based on various project parameters. The application provides detailed cost breakdowns and suggests cost-saving alternatives based on civil engineering principles.

## Features

- **Landing Page**: Brief introduction to the application and its features
- **Project Input Page**: Form to input dimensions, materials, labor hours, and other project details
- **Dashboard**: Displays total estimated cost with interactive charts/tables breaking down costs (materials, labor, overheads)
- **Cost Optimization**: Suggests alternative materials or design tweaks to reduce costs with comparative analysis
- **Report Generation**: Downloadable summary of cost estimation and recommendations
- **Estimate History**: Store and retrieve past estimations for reference

## Technologies Used

- **Frontend**: HTML5, CSS3, JavaScript, Bootstrap 5
- **Charts**: Chart.js for interactive data visualization
- **Backend**: Node.js with Express
- **Database**: MongoDB (configured but using local storage for demo)
- **PDF Generation**: PDFKit for report generation

## Setup Instructions

1. Clone the repository
2. Install dependencies:
   ```
   npm install
   ```
3. Start the server:
   ```
   npm start
   ```
4. Open your browser and navigate to `http://localhost:3000`

## Project Structure

- `index.html` - Landing page
- `estimate.html` - Project input form
- `dashboard.html` - Cost breakdown dashboard
- `optimization.html` - Cost optimization suggestions
- `history.html` - Past estimates history
- `css/styles.css` - Main stylesheet
- `js/main.js` - Main JavaScript functionality
- `js/utility.js` - Utility functions
- `server.js` - Express server and API endpoints

## Cost Calculation Logic

The application uses predefined rates for materials, labor, and equipment to calculate costs based on user inputs. The calculation includes:

1. **Material Costs**: Quantity × Unit Price for each material
2. **Labor Costs**: Hours × Hourly Rate for each labor type
3. **Equipment Costs**: Days × Daily Rate for each equipment
4. **Overhead**: Percentage of subtotal (materials + labor + equipment)
5. **Contingency**: Percentage of subtotal for unexpected costs

## Optimization Algorithms

The cost optimization feature analyzes the project details to suggest:

- Alternative materials with similar performance but lower costs
- Design optimizations to reduce material usage
- Labor scheduling improvements to increase efficiency

## Future Enhancements

- User authentication and profile management
- Integration with external APIs for real-time material pricing
- AI-based cost predictions based on historical data
- Mobile application for on-site cost estimation
- Collaboration features for team-based projects

## License

MIT License

## Contact

For any questions or feedback, please contact (atharvmahajan0205@gmail.com).
