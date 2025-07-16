<div id="#top"></div>
<br />

<p align="center">
<img src="https://github.com/vitorbritto/workflow-guide/raw/master/source/logo-wg.png" alt="Workflow Guide" width="320">
</p>

<h3 align="center">Workflow Guide</h3>

<br />
<br />
<details>
  <summary>Summary</summary>
  <ol>
    <li><a href="#workflow-lifecycle">Workflow Lifecycle</a></li>
    <li><a href="#tools">Tools</a></li>
    <li><a href="#tech-stack">Tech Stack</a></li>
    <li><a href="#guides">Guides</a></li>
    <li><a href="#best-practices">Best Practices</a></li>
  </ol>
</details>
<br />

# Introduction

Hello there! I'm Vitor Britto, a Senior Software Engineer based in Brazil with over 15 years of experience in the software industry.
I'm passionate about improving skills, learning new technologies, enjoy influencing others and always advocate for technical excellence while being open to change.
I have strong experience building SaaS applications and developing software products.

:rocket: Feel free to visit my personal website: https://vitorbritto.dev

## About this Guide

1. A personal Framework with approaches and methods that I use to delivery high-quality softwares.
2. Tools that makes my Workflow easy.
3. My own code conventions, which is inspired by what is popular within the community and flavored with some personal opinions.
4. Major dependencies that I use.

## The main reasons

- Apply rules and be based on a principle and methodology of process which could maintain the structure of my standards.
- Not only have a code style guide, but relevant informations about my Workflow. Thus I always keep the same logic process and can initiate the development of my projects without any questions when making a scaffolding, building process, automation rotines, unit testing and others tasks.

# Workflow Lifecycle

> You can find a complete list of applications, utilities, DevOps and Business Tools here: [![Stack Share](http://img.shields.io/badge/tech-stack-0690fa.svg?style=flat)](https://stackshare.io/vitorbritto/vbwebstudio)

This is a simple table with approaches and methods that I use at my Workflow lifecycle.

| Plan       | Design      | Develop     | Deploy       |
| ---------- | ----------- | ----------- | ------------ |
| Research   | Concepting  | Scaffolding | CI/CD        |
| Observe    | Prototype   | Coding      | Testing      |
| Understand | Refine      | Build       | Monitoring   |
| Analyze    | Style Guide | QA          | Optimization |
| Timeline   | Approval    | Review      | Maintenance  |

<p style="font-size: 14px;" align="right">[<a href="#top">back to top</a>]</p>

# Tools

## Plan & Project Management

- [Notion](https://notion.so/) - _Documentation and knowledge base_
- [Figma](https://www.figma.com/) - _Design and prototyping_
- [Draw.io](https://www.draw.io/) - _System architecture diagrams_

## Communication & Collaboration

- [Slack](https://slack.com/) - _Team messaging and collaboration_
- [Discord](https://discord.com/) - _Community and team communication_
- [Google Meet](https://meet.google.com/) - _Video conferencing_
- [Loom](https://loom.com/) - _Screen recording and async communication_

## Development Environment

### Code Editors & IDEs

- [Zed](https://zed.dev/) - _AI-powered code editor_

### Terminal & Shell

- [Warp](https://www.warp.dev/) - _Terminal emulator for macOS_

### Version Control

- [Git](https://git-scm.com/) - _Version control system_
- [GitHub](https://github.com/) - _Code hosting and collaboration_

<p style="font-size: 14px;" align="right">[<a href="#top">back to top</a>]</p>

# Tech Stack

## Frontend Development

### Frameworks & Libraries

- [Next.js 14+](https://nextjs.org/)
- [React 19+](https://react.dev/)

### Styling & UI

- [Tailwind CSS](https://tailwindcss.com/) - _Utility-first CSS framework_
- [Shadcn/ui](https://ui.shadcn.com/) - _Re-usable components_
- [Radix UI](https://www.radix-ui.com/) - _Unstyled, accessible components_
- [Material UI](https://mui.com/) - _React components that implement Google's Material Design_
- [Framer Motion](https://www.framer.com/motion/) - _Animation library_

### State Management

- [Zustand](https://zustand-demo.pmnd.rs/) - _Lightweight state management_
- [TanStack Query](https://tanstack.com/query) - _Server state management_
- [Redux Toolkit](https://redux-toolkit.js.org/) - _Predictable state container_

## Backend Development

### Runtime & Frameworks

- [Node.js](https://nodejs.org/)
- [Express.js](https://expressjs.com/)
- [NestJS](https://nestjs.com/)
- [Fastify](https://fastify.dev/)

### Database & ORM

- [PostgreSQL](https://www.postgresql.org/) - _Primary relational database_
- [Prisma](https://www.prisma.io/) - _Modern database toolkit_
- [MongoDB](https://www.mongodb.com/) - _NoSQL database_
- [Redis](https://redis.io/) - _In-memory data store_
- [Supabase](https://supabase.com/) - _Open source Firebase alternative_

### Authentication & Security

- [NextAuth.js](https://next-auth.js.org/) - _Authentication for Next.js_
- [Clerk](https://clerk.com/) - _User management and authentication_
- [Supertokens](https://supertokens.com/) - _Complete authentication solution_

## Mobile Development

- [React Native](https://reactnative.dev/) - _Cross-platform mobile development_
- [Expo](https://expo.dev/) - _React Native development platform_
- [Ignite](https://ignite.com/) - _React Native development platform_

## Testing

### Unit & Integration Testing

- [Vitest](https://vitest.dev/) - _Fast unit testing framework_
- [Jest](https://jestjs.io/) - _JavaScript testing framework_
- [Testing Library](https://testing-library.com/) - _Testing utilities_
- [MSW](https://mswjs.io/) - _API mocking_

### E2E Testing

- [Playwright](https://playwright.dev/) - _End-to-end testing_
- [Cypress](https://www.cypress.io/) - _Web application testing_
- [Detox](https://wix.github.io/Detox/) - _Mobile E2E testing_

## DevOps & Cloud

### Cloud Platforms

- [Vercel](https://vercel.com/) - _Deployment platform for Next.js_
- [AWS](https://aws.amazon.com/) - _Cloud computing platform_

### Infrastructure & Deployment

- [Docker](https://www.docker.com/) - _Containerization platform_
- [Kubernetes](https://kubernetes.io/) - _Container orchestration_
- [Terraform](https://www.terraform.io/) - _Infrastructure as code_
- [CDK](https://aws.amazon.com/cdk/) - _Infrastructure as code_
- [GitHub Actions](https://github.com/features/actions) - _CI/CD automation_
- [Vercel](https://vercel.com/) - _Zero-config deployments_

### Monitoring & Analytics

- [Sentry](https://sentry.io/) - _Error monitoring_
- [PostHog](https://posthog.com/) - _Product analytics_

## Development Tools

### Build Tools & Bundlers

- [Vite](https://vitejs.dev/) - _Fast build tool_
- [Turbopack](https://turbo.build/pack) - _Incremental bundler_
- [esbuild](https://esbuild.github.io/) - _Extremely fast bundler_

### Package Managers

- [pnpm](https://pnpm.io/) - _Fast, disk space efficient package manager_

### Code Quality

- [ESLint](https://eslint.org/) - _JavaScript linting_
- [Prettier](https://prettier.io/) - _Code formatter_
- [TypeScript](https://www.typescriptlang.org/) - _Typed JavaScript_
- [Husky](https://typicode.github.io/husky/) - _Git hooks_
- [lint-staged](https://github.com/okonet/lint-staged) - _Run linters on staged files_

<p style="font-size: 14px;" align="right">[<a href="#top">back to top</a>]</p>

# Guides

For web projects in which I work from planning to delivery, I use the guides below. If I am on a team that already has established guides, I'll follow the rules already adopted. No bullshit, just follow the rules.

## Project Management

- **[STRATEGY]**: Kanban and/or [Scrum](http://scrummethodology.com/) method
- **[AGILE]**: [Shape Up](https://basecamp.com/shapeup) methodology for product development
- **[PLANNING]**: [OKR](https://www.whatmatters.com/faqs/okr-meaning-definition-example/) framework for goal setting

## Development Principles

- **[ARCHITECTURE]**: Clean architecture, Clean Code and [The Twelve-factor app](https://12factor.net/)
- **[DESIGN]**: [SOLID principles](https://en.wikipedia.org/wiki/SOLID) and [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
- **[SECURITY]**: [OWASP Top 10](https://owasp.org/www-project-top-ten/) security practices
- **[PERFORMANCE]**: [Core Web Vitals](https://web.dev/vitals/) optimization

## Code Standards

- **[STYLE]**: [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- **[COMMITS]**: [Conventional Commits](https://www.conventionalcommits.org/)
- **[BRANCHING]**: [Git Flow](https://nvie.com/posts/a-successful-git-branching-model/) or [GitHub Flow](https://guides.github.com/introduction/flow/)

**Be Consistent**

> The point of having style guidelines is to have a common vocabulary of coding so people can concentrate on what you're saying rather than on how you're saying it. We present global style rules here so people know the vocabulary, but local style is also important. If code you add to a file looks drastically different from the existing code around it, it throws readers out of their rhythm when they go to read it. Avoid this.

<p style="font-size: 14px;" align="right">[<a href="#top">back to top</a>]</p>

# Best Practices

## Performance

- Use [React.memo](https://react.dev/reference/react/memo) for expensive components
- Implement [code splitting](https://react.dev/reference/react/lazy) with React.lazy
- Optimize images with [next/image](https://nextjs.org/docs/api-reference/next/image)
- Use [SWR](https://swr.vercel.app/) or [TanStack Query](https://tanstack.com/query) for data fetching
- Implement [virtual scrolling](https://github.com/bvaughn/react-window) for large lists

## Security

- Always validate input data
- Use HTTPS in production
- Implement proper CORS policies
- Sanitize user inputs
- Use environment variables for sensitive data
- Regular dependency updates

## Accessibility

- Follow [WCAG 2.1](https://www.w3.org/WAI/WCAG21/quickref/) guidelines
- Use semantic HTML elements
- Provide alt text for images
- Ensure keyboard navigation
- Test with screen readers

## SEO

- Use [next-seo](https://github.com/garmeeh/next-seo) for meta tags
- Implement structured data
- Optimize for Core Web Vitals
- Use descriptive URLs
- Create sitemaps

<p style="font-size: 14px;" align="right">[<a href="#top">back to top</a>]</p>

# License

[MIT License](http://vitorbritto.mit-license.org/) © Vitor Britto
