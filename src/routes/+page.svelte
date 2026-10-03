<script>
  const github = 'https://github.com/sukanyanath1';

  const scholar =
    'https://scholar.google.com/citations?user=WWjzvnoAAAAJ&hl=en';

  const presentations = [
    {
      title: 'Teaching presentation 1',
      previewUrl:
        'https://docs.google.com/presentation/d/1hrMPllIGBMJaxSiCayg3VY4-FPf7IhHB65coL120kPQ/embed?start=false&loop=false&delayms=3000',
      url: 'https://docs.google.com/presentation/d/1hrMPllIGBMJaxSiCayg3VY4-FPf7IhHB65coL120kPQ/edit?usp=sharing'
    },
    {
      title: 'Teaching presentation 2',
      previewUrl:
        'https://docs.google.com/presentation/d/10wctaEvJ0aplVyQNwYEFFI5lSGPgPRJqgNdrUfWVmCs/embed?start=false&loop=false&delayms=3000',
      url: 'https://docs.google.com/presentation/d/10wctaEvJ0aplVyQNwYEFFI5lSGPgPRJqgNdrUfWVmCs/edit?usp=sharing'
    },
    {
      title: 'AI Anwendungen im administrativen Bereich',
      previewUrl:
        '/presentations/AI%20Anwendungen%20im%20administrativen%20Bereich.pdf#page=1&view=FitH&toolbar=0',
      url: '/presentations/AI%20Anwendungen%20im%20administrativen%20Bereich.pdf'
    },
    {
      title: 'InformationsKiosk Seminar',
      previewUrl:
        '/presentations/Informationskiosk_Seminar_published_slides.pdf#page=1&view=FitH&toolbar=0',
      url: '/presentations/Informationskiosk_Seminar_published_slides.pdf'
    }
  ];

  const projects = [
    {
      title: 'Generative AI Platform / Bot-as-a-Service',
      description:
        'A reusable platform for deploying customer-specific RAG and agentic AI applications, with tenant-specific configuration, retrieval infrastructure, authentication, evaluation and deployment tooling.',
      role:
        'Architecture and implementation across the AI backend, retrieval layer, customer configuration, deployment infrastructure and evaluation.',
      technologies: [
        'Python',
        'FastAPI',
        'Azure AI Search',
        'RAG',
        'Agentic AI',
        'Redis',
        'Kubernetes',
        'Terraform'
      ],
      links: [
        {
          label: 'Live Site',
          url: 'http://baas.dsl.unibe.ch'
        },
        {
          label: 'GitHub',
          url: github
        }
      ]
    },
    {
      title: 'InformationsKiosk - University Information Assistant',
      description:
        'A multilingual AI assistant for answering institutional questions using verifiable university sources. The system combines retrieval, document ingestion, source attribution, evaluation, feedback and administrative tooling.',
      role:
        'Lead development across system architecture, RAG, backend APIs, evaluation, observability and productionisation.',
      technologies: [
        'LLMs',
        'RAG',
        'FastAPI',
        'Azure',
        'SvelteKit',
        'Document Processing',
        'Evaluation',
        'Playwright'
      ],
      links: [
        {
          label: 'Live Site',
          url: 'https://informationskiosk.unibe.ch'
        },
        {
          label: 'Presentation',
          url: '/presentations/Informationskiosk_Seminar_published_slides.pdf'
        },
        {
          label: 'GitHub',
          url: github
        }
      ]
    },
    {
      title: 'CLIM+ Climate Assistant',
      description:
        'AI-powered information retrieval and question answering for climate-science content, combining web and document ingestion with retrieval and conversational access to project knowledge.',
      role:
        'Designed and implemented the retrieval, ingestion and application architecture.',
      technologies: [
        'Python',
        'Generative AI',
        'RAG',
        'Web Crawling',
        'Information Retrieval'
      ],
      links: [
        {
          label: 'Live Site',
          url: 'https://climebot.dsl.unibe.ch/'
        },
        {
          label: 'GitHub',
          url: github
        }
      ]
    },
    {
      title: 'AI Research Observability',
      description:
        'Research on independently verifiable evidence for detecting epistemic degradation in autonomous research systems, including failure taxonomies, evaluation design and audit-oriented observability.',
      role:
        'Independent research and benchmark design.',
      technologies: [
        'AI Evaluation',
        'Autonomous Agents',
        'Observability',
        'Research Automation'
      ],
      links: [
        {
          label: 'Publications',
          url: scholar
        }
      ]
    }
  ];

  const skillGroups = [
    {
      title: 'Generative AI',
      items: [
        'RAG',
        'Agentic systems',
        'LLM evaluation',
        'Tool use',
        'Prompt and system design',
        'Grounded generation'
      ]
    },
    {
      title: 'AI & NLP',
      items: [
        'Python',
        'Natural Language Processing',
        'Transformers',
        'Machine Learning',
        'Information Retrieval',
      ]
    },
    {
      title: 'Cloud & Platform',
      items: [
        'Azure',
        'Kubernetes',
        'Docker',
        'Terraform',
        'API Management',
        'Entra ID',
        'CI/CD',
        'Apache Kafka',
        'Redis'
      ]
    },
    {
      title: 'Production Engineering',
      items: [
        'FastAPI',
        'Django',
        'Testing',
        'Observability',
        'Security',
        'Multi-tenancy',
        'System architecture'
      ]
    }
  ];

  const publications = [
    {
      title:
        'Using Natural Language Processing to Find Indications for Burnout with Text Classification: From Online Data to Real-World Data'
    },
    {
      title:
        'BurnoutWords — Detecting Burnout for a Clinical Setting'
    },
    {
      title:
        'Style Change Detection Using Siamese Neural Networks'
    },
    {
      title:
        'Style Change Detection by Threshold-Based and Window-Merge Clustering Methods'
    }
  ];
</script>

<main>
  <nav class="nav container">
    <a href="/" class="brand">
      <img src="/logo.png" alt="Sukanya Nath" width="52" height="52" />
    </a>

    <div class="nav-links">
      <a href="#work">Work</a>
      <a href="#engineering">Engineering</a>
      <a href="#research">Research</a>
      <a href="#about">About</a>
    </div>
  </nav>

  <section class="hero container">
    <div class="eyebrow">AI ENGINEERING · NLP · GENERATIVE AI</div>

    <h1>Sukanya Nath</h1>

    <h2>
      I build AI systems from prototype to production.
    </h2>

    <p class="hero-copy">
      AI and NLP engineer working across Generative AI, retrieval,
      agentic workflows, evaluation and cloud infrastructure.
      I design systems from architecture and implementation through
      deployment, observability and operation.
    </p>

    <div class="hero-links">
      <a
        class="button primary"
        href={github}
        target="_blank"
        rel="noreferrer"
      >
        GitHub
      </a>

      <a
        class="button secondary"
        href={scholar}
        target="_blank"
        rel="noreferrer"
      >
        Google Scholar
      </a>

      <!-- Add when ready:
      <a class="button secondary" href="/Sukanya_Nath_CV.pdf">
        CV
      </a>
      -->
    </div>
  </section>

  <section class="intro container">
    <p>
      I work at the intersection of
      <strong>AI research and production software engineering</strong>.
      My work ranges from NLP and machine-learning research to reusable
      Generative AI platforms, retrieval systems and applications used
      in real organisational environments.
    </p>
  </section>

  <section id="work" class="section container">
    <div class="section-heading">
      <span>01</span>
      <h2>Selected Work</h2>
    </div>

    <div class="projects">
      {#each projects as project}
        <article class="project-card">
          <div class="project-main">
            <h3>{project.title}</h3>

            <p class="project-description">
              {project.description}
            </p>

            <p class="role">
              <strong>My role:</strong>
              {project.role}
            </p>

            <div class="tags">
              {#each project.technologies as technology}
                <span>{technology}</span>
              {/each}
            </div>
          </div>

          <div class="project-links">
            {#each project.links as link}
              <a
                href={link.url}
                target="_blank"
                rel="noreferrer"
              >
                {link.label} ↗
              </a>
            {/each}
          </div>
        </article>
      {/each}
    </div>
  </section>

  <section id="engineering" class="section container">
    <div class="section-heading">
      <span>02</span>
      <h2>Engineering</h2>
    </div>

    <div class="skill-grid">
      {#each skillGroups as group}
        <article class="skill-card">
          <h3>{group.title}</h3>

          <ul>
            {#each group.items as item}
              <li>{item}</li>
            {/each}
          </ul>
        </article>
      {/each}
    </div>
  </section>

  <section id="research" class="section container">
    <div class="section-heading">
      <span>03</span>
      <h2>Research</h2>
    </div>

    <div class="research-layout">
      <div>
        <p class="large-copy">
          My research background is in Natural Language Processing and
          applied machine learning. My current interests include
          Generative AI, autonomous research systems, AI evaluation and
          the reliability of AI-assisted scientific workflows.
        </p>

        <a
          class="text-link"
          href={scholar}
          target="_blank"
          rel="noreferrer"
        >
          Full publication list on Google Scholar ↗
        </a>
      </div>

      <div class="publication-list">
        <h3>Selected publications</h3>

        {#each publications as publication}
          <article class="publication">
            <p>{publication.title}</p>
          </article>
        {/each}
      </div>
    </div>
  </section>

  <section class="section container">
    <div class="section-heading">
      <span>04</span>
      <h2>Teaching & Training</h2>
    </div>

    <p class="large-copy narrow">
      I teach modern NLP and Transformers and contribute to technical
      training in AI, machine learning and research software engineering.
      I particularly enjoy translating emerging AI methods into systems
      and practices that other researchers and engineers can use. In addition
      to the selected presentations, I am also a module lecturer for the
      <a
        class="text-link"
        href="https://www.unibe.ch/continuing_education_programs/cas_natural_language_processing/index_eng.html#collapse_pane1290197"
        target="_blank"
        rel="noreferrer"
      >CAS in Natural Language Processing ↗</a>.
    </p>

    <div class="presentations">
      {#each presentations as presentation}
        <article class="presentation-preview">
          <iframe
            src={presentation.previewUrl}
            title={presentation.title}
            loading="lazy"
            allowfullscreen
          ></iframe>

          <a
            class="text-link"
            href={presentation.url}
            target="_blank"
            rel="noreferrer"
          >
            {presentation.title} ↗
          </a>
        </article>
      {/each}
    </div>
  </section>

  <section id="about" class="section container">
    <div class="section-heading">
      <span>05</span>
      <h2>About</h2>
    </div>

    <div class="about">
    <p>
        <a
          class="text-link"
          href="https://www.dsl.unibe.ch/about/people_metadata/dr_nath_sukanya/"
          target="_blank"
          rel="noreferrer"
        >University of Bern profile ↗</a>
      </p>
      <p>
        I am an AI engineer and researcher based in Bern, Switzerland.
      </p>

      <p>
        I am particularly interested in systems that need to move beyond
        demonstrations: AI systems that have to be evaluated, deployed,
        secured, observed and maintained for real users.
      </p>

      <p>
        My work combines machine learning and NLP with backend
        engineering, cloud infrastructure and system architecture.
      </p>

      <p>
        My background is in AI/ NLP/ Computer Science/Data Science.  
      </p>
      
      <p>
      When I am not working, I am being a <strong>mum</strong> to a curious child. 
      </p>

    </div>
  </section>

  <footer class="footer container">
    <div>
      <strong>Sukanya Nath</strong>
      <p>AI / NLP Engineer · Bern, Switzerland</p>
    </div>

    <div class="footer-links">
      <a href={github} target="_blank" rel="noreferrer">
        GitHub
      </a>

      <a href={scholar} target="_blank" rel="noreferrer">
        Scholar
      </a>
    </div>
  </footer>
</main>