<div style="display: flex; flex-direction: column; gap: 15px; margin-top: 20px;">
  {{ range .Page.Pages }}
    <a href="{{ .RelPermalink }}" style="text-decoration: none; color: inherit;">
      <div style="border: 1px solid #2a2a2a; border-radius: 12px; padding: 20px; background-color: #121212;">
        <h3 style="margin: 0 0 8px 0; font-size: 1.25rem; font-weight: 600; color: #fff;">{{ .Title }}</h3>
        <p style="margin: 0; color: #a0a0a0; font-size: 0.95rem;">
          {{ if .Date }}<span style="color: #888;">{{ .Date.Format "02/01/2006" }}</span> — {{ end }}{{ .Params.description }}
        </p>
      </div>
    </a>
  {{ end }}
</div>