import React, { useState } from "react";
<Input label="Utente" placeholder="nome.cognome" />
<Input label="Password" type="password" placeholder="••••••••" />
<button type="button" className="inline-flex items-center gap-2 rounded-2xl px-4 py-2 bg-white shadow hover:shadow-md">
<LogIn className="w-4 h-4"/> Accedi
</button>
</form>
</Card>
</main>


<div className="max-w-6xl mx-auto px-4 pb-10">
<button onClick={goPublic} className="underline">← Torna alla pagina pubblica</button>
</div>
</div>
);
}


function HeroCard() {
return (
<div className="bg-white rounded-3xl shadow p-6 md:p-8">
<div className="flex items-center gap-3 mb-4">
<Ambulance className="w-6 h-6" />
<h3 className="font-semibold">Punti chiave</h3>
</div>
<ul className="space-y-2 text-blue-700/80">
<li>• Croce ben visibile e logo centrale</li>
<li>• Servizi principali subito in evidenza</li>
<li>• Prenotazione rapida e contatto immediato</li>
<li>• Seconda pagina riservata per il personale</li>
</ul>
</div>
);
}


function Card({ title, children }: { title: string; children: React.ReactNode }) {
return (
<div className="bg-white rounded-2xl shadow p-5">
<h3 className="font-semibold mb-2 flex items-center gap-2"><Shield className="w-4 h-4"/>{title}</h3>
{children}
</div>
);
}


function Input({ label, className = "", ...props }: React.InputHTMLAttributes<HTMLInputElement> & { label: string; className?: string }) {
return (
<label className={`text-sm grid gap-1 ${className}`}>
<span className="opacity-80">{label}</span>
<input {...props} className="rounded-xl border border-pink-100 bg-pink-50 px-3 py-2 focus:outline-none focus:ring-2 focus:ring-pink-200" />
</label>
);
}


function Textarea({ label, className = "", ...props }: React.TextareaHTMLAttributes<HTMLTextAreaElement> & { label: string; className?: string }) {
return (
<label className={`text-sm grid gap-1 ${className}`}>
<span className="opacity-80">{label}</span>
<textarea {...props} className="rounded-xl border border-pink-100 bg-pink-50 px-3 py-2 min-h-[100px] focus:outline-none focus:ring-2 focus:ring-pink-200" />
</label>
);
}


function Select({ label, options, className = "", ...props }: { label: string; options: string[]; className?: string } & React.SelectHTMLAttributes<HTMLSelectElement>) {
return (
<label className={`text-sm grid gap-1 ${className}`}>
<span className="opacity-80">{label}</span>
<select {...props} className="rounded-xl border border-pink-100 bg-pink-50 px-3 py-2 focus:outline-none focus:ring-2 focus:ring-pink-200">
{options.map((opt) => (
<option key={opt} value={opt}>{opt}</option>
))}
</select>
</label>
);
}


function PatientRow({ name, mobility, floor, elevator, oxygen }: { name: string; mobility: string; floor: string; elevator: string; oxygen: string }) {
return (
<div className="p-3 rounded-xl bg-pink-50 border border-pink-100">
<div className="font-medium">{name}</div>
<div className="text-sm opacity-80">Mobilità: {mobility} • Piano: {floor} • Ascensore: {elevator} • Ossigeno: {oxygen}</div>
</div>
);
}
