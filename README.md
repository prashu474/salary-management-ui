# Salary Management UI (Frontend)

## 🏗️ Architecture
- **Framework**: Next.js 14 with App Router
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **State Management**: TanStack Query (React Query)
- **Key Features**:
  - Server-side rendering for performance
  - Responsive design
  - Real-time search and filtering
  - Paginated employee lists

## 🚀 Getting Started

### Prerequisites
- Node.js 18+
- npm

### Frontend Setup
```bash
cd salary-management-ui

npm install

# Set environment variable
echo "NEXT_PUBLIC_API_URL=http://localhost:3001/api/v1" > .env.local

npm run dev
```

### Access
- **Frontend**: http://localhost:3000

## ✅ Frontend Features
- Dashboard with key metrics
- Employee list with search and filtering
- Pagination (50 records per page)
- Status filtering (active, on_leave, terminated)
- Salary insights by country
- Salary insights by job title
- Responsive design
- TypeScript for type safety
- React Query for efficient data fetching

## 🎨 User Interface

### Dashboard
- Total employees count
- Average salary
- Average tenure
- Recent hires (last 30 days)
- Quick access to employees and insights
- Recent employees table preview

### Employees Page
- Sortable, filterable table
- Search across name, email, employee ID
- Status filter
- Pagination controls
- Displays: name, job title, department, location, salary, tenure, status

### Insights Page
- Salary statistics by country table
- Salary statistics by job title table
- Min/max/average salary breakdowns
- Employee counts per category

## 🔧 Technical Decisions
1. **Next.js App Router**: Modern routing with better performance
2. **TanStack Query**: Automatic caching and refetching
3. **Tailwind CSS**: Utility-first CSS for rapid development
4. **TypeScript**: Type safety and better developer experience
5. **Component Reusability**: Shared utility functions for formatting

## 🗂️ Project Structure
```
salary-management-ui/
├── app/
│   ├── page.tsx                # Dashboard
│   ├── employees/
│   │   └── page.tsx            # Employee list
│   └── insights/
│       └── page.tsx            # Insights dashboard
├── components/
│   └── providers/
│       └── query-provider.tsx
├── lib/
│   ├── api.ts                  # API client
│   └── utils.ts                # Utility functions
└── package.json
```

## 🧪 Testing
```bash
cd salary-management-ui
npm test
```

## 🚢 Deployment (Vercel)
```bash
cd salary-management-ui
vercel --prod
```

## 📝 Environment Variables
```
NEXT_PUBLIC_API_URL=https://your-api-url.com/api/v1
```
