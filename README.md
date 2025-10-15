# front end project 
import React, { useEffect, useMemo, useState } from "react";

{e.department} • {e.location}
Joined: {e.joinedAt}
{e.email}
{e.phone}
))}
{/* pagination */}

setPage(p=>Math.max(1,p-1))} className="px-3 py-1 border rounded disabled:opacity-50">Prev
Page {page} / {totalPages}
=totalPages} onClick={()=>setPage(p=>Math.min(totalPages,p+1))} className="px-3 py-1 border rounded disabled:opacity-50">Next
{/* modal - employee details */} {selected && (

setSelected(null)}>
e.stopPropagation()}>
{initials(selected.name)}
{selected.name}
{selected.title} — {selected.department}
{selected.location} • Joined {selected.joinedAt}
{selected.bio}
Email: {selected.email}
Phone: {selected.phone}
{ navigator.clipboard?.writeText(selected.email); }} className="px-3 py-2 border rounded">Copy Email setSelected(null)} className="px-3 py-2 bg-indigo-600 text-white rounded">Close
)}
{/* small footer with quick tips */}

Tip: Click any card to view more details. Replace mock data with API calls for real data. ); }
