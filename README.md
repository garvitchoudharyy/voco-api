# Voco AI - made by Garvit

A web coding agent. Describe an app, Voco creates every file, shows a live preview for websites,
and lets you download the project as a ZIP.

## Deploy to Vercel
1. Put this folder on GitHub, then on vercel.com click Add New -> Project and import it (or run `npx vercel --prod` here).
2. Add Environment Variables, then Deploy (redeploy after changing them):
   - `VOCO_BASE_URL` - any OpenAI-compatible endpoint ending in /v1, publicly reachable
   - `VOCO_API_KEY`  - the key for that endpoint
   - `VOCO_MODEL`    - a model that supports tool/function calling
   - `VOCO_ACCESS_CODE` - (recommended) a password you choose
3. Open your .vercel.app URL and start building.

## Which endpoint?
- Your own OmniRoute hosted on a public server: `https://your-server/v1`, model `auto/coding`
  (localhost will NOT work from Vercel).
- Or a provider with a free tier: Groq `https://api.groq.com/openai/v1`,
  OpenRouter `https://openrouter.ai/api/v1`, Google Gemini `https://generativelanguage.googleapis.com/v1beta/openai`.
  Check the provider's model list for one that supports tool calling.
# voco-api
