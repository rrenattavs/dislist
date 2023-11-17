<h1>Project DSList Game</h1>
<h2>Description: </h2>
<p>This model is a system for managing lists of Games</p>

<h2>Domain Model</h2>
<img src="https://i.ibb.co/GHYSD6G/dslist-model.png" alt="dslist-model" width="824" height="290" data-is360="0" data-load="full" class="" style="width: 791px; height: 278.386px; display: block;">

<!--Code snippets configuration on the Spring boot files-->

<h2>Code Snippets</h2>
<h3>Plug-in Maven</h3>
<div class="highlight highlight-text-xml notranslate position-relative overflow-auto" dir="auto"><pre>&lt;<span class="pl-ent">plugin</span>&gt;
	&lt;<span class="pl-ent">groupId</span>&gt;org.apache.maven.plugins&lt;/<span class="pl-ent">groupId</span>&gt;
	&lt;<span class="pl-ent">artifactId</span>&gt;maven-resources-plugin&lt;/<span class="pl-ent">artifactId</span>&gt;
	&lt;<span class="pl-ent">version</span>&gt;3.1.0&lt;/<span class="pl-ent">version</span>&gt; <span class="pl-c"><span class="pl-c">&lt;!--</span>$NO-MVN-MAN-VER$ <span class="pl-c">--&gt;</span></span>
&lt;/<span class="pl-ent">plugin</span>&gt;</pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="<plugin>
	<groupId>org.apache.maven.plugins</groupId>
	<artifactId>maven-resources-plugin</artifactId>
	<version>3.1.0</version> <!--$NO-MVN-MAN-VER$ -->
</plugin>" tabindex="0" role="button" style="display: none;">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h3>application.properties</h3>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>spring.profiles.active=${APP_PROFILE:test}
spring.jpa.open-in-view=false

cors.origins=${CORS_ORIGINS:http://localhost:5173,http://localhost:3000}
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="spring.profiles.active=${APP_PROFILE:test}
spring.jpa.open-in-view=false

cors.origins=${CORS_ORIGINS:http://localhost:5173,http://localhost:3000}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h3>application-test.properties</h3>
<div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code># H2 Connection
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.username=sa
spring.datasource.password=

# H2 Client
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console

# Show SQL
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="# H2 Connection
spring.datasource.url=jdbc:h2:mem:testdb
spring.datasource.username=sa
spring.datasource.password=

# H2 Client
spring.h2.console.enabled=true
spring.h2.console.path=/h2-console

# Show SQL
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
  <h3>application-dev.properties</h3>
  <div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>#spring.jpa.properties.jakarta.persistence.schema-generation.create-source=metadata
#spring.jpa.properties.jakarta.persistence.schema-generation.scripts.action=create
#spring.jpa.properties.jakarta.persistence.schema-generation.scripts.create-target=create.sql
#spring.jpa.properties.hibernate.hbm2ddl.delimiter=;

spring.datasource.url=jdbc:postgresql://localhost:5432/dscatalog
spring.datasource.username=postgres
spring.datasource.password=1234567

spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation=true
spring.jpa.hibernate.ddl-auto=none
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="#spring.jpa.properties.jakarta.persistence.schema-generation.create-source=metadata
#spring.jpa.properties.jakarta.persistence.schema-generation.scripts.action=create
#spring.jpa.properties.jakarta.persistence.schema-generation.scripts.create-target=create.sql
#spring.jpa.properties.hibernate.hbm2ddl.delimiter=;

spring.datasource.url=jdbc:postgresql://localhost:5432/dscatalog
spring.datasource.username=postgres
spring.datasource.password=1234567

spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation=true
spring.jpa.hibernate.ddl-auto=none" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success m-2 d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
  <h3>application-prod.properties</h3>
  <div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>spring.datasource.url=${DB_URL}
spring.datasource.username=${DB_USERNAME}
spring.datasource.password=${DB_PASSWORD}

spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation=true
spring.jpa.hibernate.ddl-auto=none
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="spring.datasource.url=${DB_URL}
spring.datasource.username=${DB_USERNAME}
spring.datasource.password=${DB_PASSWORD}

spring.jpa.database-platform=org.hibernate.dialect.PostgreSQLDialect
spring.jpa.properties.hibernate.jdbc.lob.non_contextual_creation=true
spring.jpa.hibernate.ddl-auto=none" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
  <h3>system.properties</h3>
  <div class="snippet-clipboard-content notranslate position-relative overflow-auto"><pre class="notranslate"><code>java.runtime.version=17
</code></pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="java.runtime.version=17" tabindex="0" role="button" style="display: inherit;">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>

  <h3>WebConfig</h3>
  <div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">@</span><span class="pl-c1">Configuration</span>
<span class="pl-k">public</span> <span class="pl-k">class</span> <span class="pl-smi">WebConfig</span> {

	<span class="pl-c1">@</span><span class="pl-c1">Value</span>(<span class="pl-s">"${cors.origins}"</span>)
	<span class="pl-k">private</span> <span class="pl-smi">String</span> <span class="pl-s1">corsOrigins</span>;
	
	<span class="pl-c1">@</span><span class="pl-c1">Bean</span>
	<span class="pl-k">public</span> <span class="pl-smi">WebMvcConfigurer</span> <span class="pl-en">corsConfigurer</span>() {
		<span class="pl-k">return</span> <span class="pl-k">new</span> <span class="pl-smi">WebMvcConfigurer</span>() {
			<span class="pl-c1">@</span><span class="pl-c1">Override</span>
			<span class="pl-k">public</span> <span class="pl-smi">void</span> <span class="pl-en">addCorsMappings</span>(<span class="pl-smi">CorsRegistry</span> <span class="pl-s1">registry</span>) {
				<span class="pl-s1">registry</span>.<span class="pl-en">addMapping</span>(<span class="pl-s">"/**"</span>).<span class="pl-en">allowedMethods</span>(<span class="pl-s">"*"</span>).<span class="pl-en">allowedOrigins</span>(<span class="pl-s1">corsOrigins</span>);
			}
		};
	}
	
}</pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@Configuration
public class WebConfig {

	@Value(&quot;${cors.origins}&quot;)
	private String corsOrigins;
	
	@Bean
	public WebMvcConfigurer corsConfigurer() {
		return new WebMvcConfigurer() {
			@Override
			public void addCorsMappings(CorsRegistry registry) {
				registry.addMapping(&quot;/**&quot;).allowedMethods(&quot;*&quot;).allowedOrigins(corsOrigins);
			}
		};
	}
	
}" tabindex="0" role="button" style="display: inherit;">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
  <h3>GameRepository</h3>
  <div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">@</span><span class="pl-c1">Query</span>(<span class="pl-s1">nativeQuery</span> = <span class="pl-c1">true</span>, <span class="pl-s1">value</span> = <span class="pl-s">"""</span>
<span class="pl-s">		SELECT tb_game.id, tb_game.title, tb_game.game_year AS `year`, tb_game.img_url AS imgUrl,</span>
<span class="pl-s">		tb_game.short_description AS shortDescription, tb_belonging.position</span>
<span class="pl-s">		FROM tb_game</span>
<span class="pl-s">		INNER JOIN tb_belonging ON tb_game.id = tb_belonging.game_id</span>
<span class="pl-s">		WHERE tb_belonging.list_id = :listId</span>
<span class="pl-s">		ORDER BY tb_belonging.position</span>
<span class="pl-s">			"""</span>)
<span class="pl-smi">List</span>&lt;<span class="pl-smi">GameMinProjection</span>&gt; <span class="pl-s1">searchByList</span>(<span class="pl-smi">Long</span> <span class="pl-s1">listId</span>);</pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@Query(nativeQuery = true, value = &quot;&quot;&quot;
		SELECT tb_game.id, tb_game.title, tb_game.game_year AS `year`, tb_game.img_url AS imgUrl,
		tb_game.short_description AS shortDescription, tb_belonging.position
		FROM tb_game
		INNER JOIN tb_belonging ON tb_game.id = tb_belonging.game_id
		WHERE tb_belonging.list_id = :listId
		ORDER BY tb_belonging.position
			&quot;&quot;&quot;)
List<GameMinProjection> searchByList(Long listId);" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
  <h3>GameListRepository</h3>
  <div class="highlight highlight-source-java notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-c1">@</span><span class="pl-c1">Modifying</span>
<span class="pl-c1">@</span><span class="pl-c1">Query</span>(<span class="pl-s1">nativeQuery</span> = <span class="pl-c1">true</span>, <span class="pl-s1">value</span> = <span class="pl-s">"UPDATE tb_belonging SET position = :newPosition WHERE list_id = :listId AND game_id = :gameId"</span>)
<span class="pl-smi">void</span> <span class="pl-s1">updateBelongingPosition</span>(<span class="pl-smi">Long</span> <span class="pl-s1">listId</span>, <span class="pl-smi">Long</span> <span class="pl-s1">gameId</span>, <span class="pl-smi">Integer</span> <span class="pl-s1">newPosition</span>);</pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="@Modifying
@Query(nativeQuery = true, value = &quot;UPDATE tb_belonging SET position = :newPosition WHERE list_id = :listId AND game_id = :gameId&quot;)
void updateBelongingPosition(Long listId, Long gameId, Integer newPosition);" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
  <h3>import.sql</h3>
  <div class="highlight highlight-source-sql notranslate position-relative overflow-auto" dir="auto"><pre><span class="pl-k">INSERT INTO</span> tb_game_list (name) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Aventura e RPG<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game_list (name) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Jogos de plataforma<span class="pl-pds">'</span></span>);

<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Mass Effect Trilogy<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>.<span class="pl-c1">8</span>, <span class="pl-c1">2012</span>, <span class="pl-s"><span class="pl-pds">'</span>Role-playing (RPG), Shooter<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>XBox, Playstation, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/1.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Red Dead Redemption 2<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>.<span class="pl-c1">7</span>, <span class="pl-c1">2018</span>, <span class="pl-s"><span class="pl-pds">'</span>Role-playing (RPG), Adventure<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>XBox, Playstation, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/2.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>The Witcher 3: Wild Hunt<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>.<span class="pl-c1">7</span>, <span class="pl-c1">2014</span>, <span class="pl-s"><span class="pl-pds">'</span>Role-playing (RPG), Adventure<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>XBox, Playstation, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/3.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Sekiro: Shadows Die Twice<span class="pl-pds">'</span></span>, <span class="pl-c1">3</span>.<span class="pl-c1">8</span>, <span class="pl-c1">2019</span>, <span class="pl-s"><span class="pl-pds">'</span>Role-playing (RPG), Adventure<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>XBox, Playstation, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/4.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Ghost of Tsushima<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>.<span class="pl-c1">6</span>, <span class="pl-c1">2012</span>, <span class="pl-s"><span class="pl-pds">'</span>Role-playing (RPG), Adventure<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>XBox, Playstation, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/5.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Super Mario World<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>.<span class="pl-c1">7</span>, <span class="pl-c1">1990</span>, <span class="pl-s"><span class="pl-pds">'</span>Platform<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Super Ness, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/6.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Hollow Knight<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>.<span class="pl-c1">6</span>, <span class="pl-c1">2017</span>, <span class="pl-s"><span class="pl-pds">'</span>Platform<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>XBox, Playstation, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/7.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Ori and the Blind Forest<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>, <span class="pl-c1">2015</span>, <span class="pl-s"><span class="pl-pds">'</span>Platform<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>XBox, Playstation, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/8.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Cuphead<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>.<span class="pl-c1">6</span>, <span class="pl-c1">2017</span>, <span class="pl-s"><span class="pl-pds">'</span>Platform<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>XBox, Playstation, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/9.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);
<span class="pl-k">INSERT INTO</span> tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) <span class="pl-k">VALUES</span> (<span class="pl-s"><span class="pl-pds">'</span>Sonic CD<span class="pl-pds">'</span></span>, <span class="pl-c1">4</span>, <span class="pl-c1">1993</span>, <span class="pl-s"><span class="pl-pds">'</span>Platform<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Sega CD, PC<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/10.png<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!<span class="pl-pds">'</span></span>, <span class="pl-s"><span class="pl-pds">'</span>Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.<span class="pl-pds">'</span></span>);

<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">1</span>, <span class="pl-c1">1</span>, <span class="pl-c1">0</span>);
<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">1</span>, <span class="pl-c1">2</span>, <span class="pl-c1">1</span>);
<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">1</span>, <span class="pl-c1">3</span>, <span class="pl-c1">2</span>);
<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">1</span>, <span class="pl-c1">4</span>, <span class="pl-c1">3</span>);
<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">1</span>, <span class="pl-c1">5</span>, <span class="pl-c1">4</span>);

<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">2</span>, <span class="pl-c1">6</span>, <span class="pl-c1">0</span>);
<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">2</span>, <span class="pl-c1">7</span>, <span class="pl-c1">1</span>);
<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">2</span>, <span class="pl-c1">8</span>, <span class="pl-c1">2</span>);
<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">2</span>, <span class="pl-c1">9</span>, <span class="pl-c1">3</span>);
<span class="pl-k">INSERT INTO</span> tb_belonging (list_id, game_id, position) <span class="pl-k">VALUES</span> (<span class="pl-c1">2</span>, <span class="pl-c1">10</span>, <span class="pl-c1">4</span>);</pre><div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w" value="INSERT INTO tb_game_list (name) VALUES ('Aventura e RPG');
INSERT INTO tb_game_list (name) VALUES ('Jogos de plataforma');

INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Mass Effect Trilogy', 4.8, 2012, 'Role-playing (RPG), Shooter', 'XBox, Playstation, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/1.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Red Dead Redemption 2', 4.7, 2018, 'Role-playing (RPG), Adventure', 'XBox, Playstation, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/2.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('The Witcher 3: Wild Hunt', 4.7, 2014, 'Role-playing (RPG), Adventure', 'XBox, Playstation, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/3.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Sekiro: Shadows Die Twice', 3.8, 2019, 'Role-playing (RPG), Adventure', 'XBox, Playstation, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/4.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Ghost of Tsushima', 4.6, 2012, 'Role-playing (RPG), Adventure', 'XBox, Playstation, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/5.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Super Mario World', 4.7, 1990, 'Platform', 'Super Ness, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/6.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Hollow Knight', 4.6, 2017, 'Platform', 'XBox, Playstation, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/7.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Ori and the Blind Forest', 4, 2015, 'Platform', 'XBox, Playstation, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/8.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Cuphead', 4.6, 2017, 'Platform', 'XBox, Playstation, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/9.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');
INSERT INTO tb_game (title, score, game_year, genre, platforms, img_url, short_description, long_description) VALUES ('Sonic CD', 4, 1993, 'Platform', 'Sega CD, PC', 'https://raw.githubusercontent.com/devsuperior/java-spring-dslist/main/resources/10.png', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit esse officiis corrupti unde repellat non quibusdam! Id nihil itaque ipsum!', 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Delectus dolorum illum placeat eligendi, quis maiores veniam. Incidunt dolorum, nisi deleniti dicta odit voluptatem nam provident temporibus reprehenderit blanditiis consectetur tenetur. Dignissimos blanditiis quod corporis iste, aliquid perspiciatis architecto quasi tempore ipsam voluptates ea ad distinctio, sapiente qui, amet quidem culpa.');

INSERT INTO tb_belonging (list_id, game_id, position) VALUES (1, 1, 0);
INSERT INTO tb_belonging (list_id, game_id, position) VALUES (1, 2, 1);
INSERT INTO tb_belonging (list_id, game_id, position) VALUES (1, 3, 2);
INSERT INTO tb_belonging (list_id, game_id, position) VALUES (1, 4, 3);
INSERT INTO tb_belonging (list_id, game_id, position) VALUES (1, 5, 4);

INSERT INTO tb_belonging (list_id, game_id, position) VALUES (2, 6, 0);
INSERT INTO tb_belonging (list_id, game_id, position) VALUES (2, 7, 1);
INSERT INTO tb_belonging (list_id, game_id, position) VALUES (2, 8, 2);
INSERT INTO tb_belonging (list_id, game_id, position) VALUES (2, 9, 3);
INSERT INTO tb_belonging (list_id, game_id, position) VALUES (2, 10, 4);" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<h2>Technologies</h2>
<ul>
  <li>Java</li>
  <li>Spring Boot</li>
  <li>Maven</li>
<li>Hibernate</li>
<li>SQL</li>
  <li>React.js</li>
  
</ul>
